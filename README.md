# Freshchat Live Chat Google Analytics Tracking / Facebook Pixel Event Tracking
Freshchat Live Chat Google Analytics & Facebook Pixel event tracking

This code will automatically check whether there are Facebook Pixel or Google Analytics (`analytics.js/ga` or `gtag.js`).
If the initial tracking code exists, it will send event signals to each tracking tool. 

Copy the whole code from `<script>` to `</script>` and put it in every page that has Freshchat Live Chat widget; put the code inside `<body> </body>`, preferably right before `</body>`.

Check if the code working in Google Analytics > Real Time > Events.
The live chat events tracked by this code is:
1. `widget:opened`
2. `widget:closed`
3. `message:received`
4. `message:sent`
5. `user:statechange`
6. `user:created`
7. `user:loaded`
8. `user:identified`
9. `user:restored`

To check if it works in Facebook Pixel, find the "Test Event" menu in Facebook Pixel Analytics.
The code choose `user:created` event as a Facebook Pixel `Lead` standard event.
We find it as the event that is usually triggered after a first message sent by a new user, or after the user gave email or phone number.
Just check the right event in the "Test Event" menu in Pixel Analytics and modify the code accordingly, e.g. change parameter `fb_event` to another standard event or a custom event.

The code is roughly based on <a href="https://support.freshchat.com/support/solutions/articles/238128-freshchat-with-google-analytics-event-tracking">this support article by Freshchat</a>.
