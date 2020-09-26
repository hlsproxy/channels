# HLS-Proxy (from 7.1.0)

(You can download HLS-Proxy from the official site: https://www.hls-proxy.com/)

## Setup channels match and logo replacing

HLS-Proxy has its own copy of channels.json
But, you might have to customize it for your needs.

In this case you just put channels.json along with hls-proxy executable and when HLS-Proxy will start next time it will take your copy of channels.json instead of a built-in one.

Also, you might be interested to replace channels logo.
It can be done by creating html folder and then logos folder in it and then you need to put all needed files into ./html/logos folder.

## Installation

1. Go to HLS-Proxy installation/running folder
2. Run a command: 

```bash
curl -LO https://github.com/hlsproxy/channels/archive/master.zip ; unzip -o master.zip -d "./" ; rsync -arv ./channels-master/ ./; rm -r channels-master master.zip
```

## Requirements of a channels.json format
- `_id` value should be unique
- `country` should be standard ISO 3166-1 Alpha-2 code lower case  
You can find all codes here: https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes
- `logo_url` is a link or a relative path (in case of local file) like this /logos/file.png
- `group` a one of ids from groups.json file (You can find it in HLS-Proxy package)
- `basealias`* is the main alias
- `aliases`* is string of aliases separated by `|` character

*) `basealias` and `aliases` are constructed from all possible names.  
Values for these fields should be in lowercase without spaces. Only letters and `+` allowed. All other chars should be removed.
 
## Any contributions are more than welcome
