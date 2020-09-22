# HLS-Proxy (from 7.1.0)
## Setup channels match and logo replacing

HLS-Proxy has its own copy of channels.json
But you might have to customize it for your needs.

In this case you just put channels.json along with hls-proxy executable and when HLS-Proxy will start next time it will take your copy of channels.json instead of a built-in one.

Also, you might be interested to replace channels logo.
It can be done by creating html folder and then logos folder in it and then you need to put all needed files into ./html/logos folder.

## Installation

1. Go to HLS-Proxy installation/running folder
2. Run a command: 

```bash
curl -LO https://github.com/hlsproxy/channels/archive/master.zip ; unzip -o master.zip -d "./" ; rsync -arv ./channels-master/ ./; rm -r channels-master master.zip
```
