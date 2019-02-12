# Freshchat Live Chat Google Tracking
Freshchat Live Chat Google Analytics (ga or gtag.js) event tracking

First, check if the website has analytics.js ("ga") or gtag.js for Google Analytics tracking.
Use code in freshchat_tracking_ga.html for ga tracking, freshchat_tracking_gtag.html for gtag tracking.

Copy the whole code from \<script\> to \<\/script\> and put it in every page that has Freshchat Live Chat widget; put the code inside \<body\> \<\/body\>, preferably right before \<\/body\>.

Check if the code working in Google Analytics > Real Time > Events.
The live chat events tracked by this code is:
1. widget:opened
2. widget:closed
3. message:received
4. message:sent
5. user:statechange
6. user:loaded
7. user:identified
8. user:restored

The code is roughly based on <a href="https://support.freshchat.com/support/solutions/articles/238128-freshchat-with-google-analytics-event-tracking">this support article by Freshchat</a>.
