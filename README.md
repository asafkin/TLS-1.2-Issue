# TLS-1.2-Issue
This sample app reproduces an issue communicating with a TLS 1.2 backend.

It contains a single webview thats loads a url for a website that enforces TLS 1.2. 
The issue occurs on devices with OS 4.0.
The url will not be loaded and the error received is "error = -11 description = Couldn't establish a secure connection".

This is only one case where this issue occurs. 
On network connections via OkHttp another error is received - "HTTP FAILED: javax.net.ssl.SSLException: Connection closed by peer"
