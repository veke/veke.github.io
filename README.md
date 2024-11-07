# veke.github.io
Test HTTP2 request polling using XHR or fetch using iOS 18 Safari

Steps to reproduce the issue:

Navigate to: https://veke.github.io
Note: Requires iOS 18 Safari

Start polling using XHR or fetch.
Wait response and put Safari on the background, wait 3 seconds, put Safari on foreground, observe request pending.
Repeat if not happening.
You might need perfect timing when the appswitch is done. Play around the appswitch and observe that request is stalling.

![alt text](https://github.com/veke/veke.github.io/blob/main/pending1.png)

![alt text](https://github.com/veke/veke.github.io/blob/main/pending4.png)
