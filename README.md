# HLS-Proxy (from 7.0.8)
## Setup channels match and logo replacing

HLS-Proxy has its own copy of channels.json
But you might have to customize it for your needs.

In this case you just put channels.json along with hls-proxy executable and when HLS-Proxy will start next time it will take your copy of channels.json instead a built-in one.

Also, you might be interested to replace channels logo.
It can be done by creating html folder and then logos folder in it and then you need to put all needed files into ./html/logos folder.
