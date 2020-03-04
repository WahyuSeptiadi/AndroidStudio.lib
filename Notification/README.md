# Notification
## Basic code 
**1. DefaultSound**
  - static Uri defaultSound = RingtoneManager.getDefaultUri(RingtoneManager.TYPE_NOTIFICATION);<br>

**2. DefaultNotification**
  - Notification notif = new NotificationCompat.Builder(this, CHANNEL_1_ID)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .setSmallIcon(R.drawable.ic_notification)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .setContentTitle(title)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .setContentText(deskripsi)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .setSound(defaultSound)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .addAction(replyAction)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .setPriority(NotificationCompat.PRIORITY_LOW)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .setAutoCancel(true)<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  .build();<br>
  
**3. Add Action "Reply"**
  - NotificationCompat.Action replyAction = new NotificationCompat.Action.Builder(<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  R.drawable.ic_reply,<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
  "Reply",<br>
  &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;                 replyPendingIntent).addRemoteInput(remoteInput).build();
  
  
<!--&ensp; TAB 1 -->

## Display Notification
[Big Content API 22](./ss.img/Big%20Content%20API%2022.jpeg) <br>
[Can't reply chat API 22](./ss.img/Can't%20reply%20chat%20API%2022.jpeg) <br>
[Media Player API 22](./ss.img/Media%20Player%20API%2022.jpeg) <br>
[Progress Download API 22](./ss.img/Progress%20Download%20API%2022.jpeg) <br>
[Multichat API 22](./ss.img/multichat%20API%2022.jpeg) <br>
[Reply chat API 29](./ss.img/reply%20chat%20API%2029.jpeg) <br>
[Setting notif API 26 keatas](./ss.img/setting%20notif%20API%2026%20keatas.jpeg) <br>
