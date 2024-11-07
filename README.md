# veke.github.io
Test Safari HTTP2 request polling using XHR or fetch using iOS 18

Steps to reproduce the issue:

Start polling using XHR or fetch.
Wait couple of rounds to complete requests.
After some successful responses put Safari into background, wait couple of seconds and put Safari back to foreground.
Request that is sent after Safari is put back to foreground might start pending and never finishes. 
You might need perfect timing when the appswitch is done. Play around the appswitch and observe that request is stalling.



