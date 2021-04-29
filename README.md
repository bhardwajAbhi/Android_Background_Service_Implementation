<b>How to make an Android Service to run in the background reliably every N seconds even when the device is idle.</b>

<b>The Idea is the following:</b>
Instead of creating a repeating alarm which does not respect the 15 second limit we create an exact alarm that is allowed with the idle state. The trick is that every time the alarm goes off, we set it again 15 seconds later! We created a background service which runs every 15 seconds and make a Toast !!
