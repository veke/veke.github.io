# veke.github.io
Test HTTP2 request polling using XHR or fetch using iOS 18 Safari

Steps to reproduce the issue:

Start polling using XHR or fetch.
Wait couple of rounds to complete requests.
After some successful responses put Safari into background, wait couple of seconds and put Safari back to foreground.
Request that is sent after Safari is put back to foreground might start pending and never finishes. 
You might need perfect timing when the appswitch is done. Play around the appswitch and observe that request is stalling.

![alt text](https://github.com/veke/veke.github.io/blob/main/pending.png)

![alt text](https://github.com/veke/veke.github.io/blob/main/pending2.png)
