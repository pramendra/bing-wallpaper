# Automate your Mac's background with Bing Wallpaper

## Setup

### 1. Create a shell file
```bash
$ mkdir ~/bing-wallpaer
$ touch bing-wallpaper.sh
```

### 2. add following in bing-wallpaper.sh
```
#!/bin/sh
npx bing-wallpaper-daily-mac-multimonitor
```
> using npx to fetch bing wallpaper


### 3. change the file mode
```bash
$ chmod u+x bing-wallpaper.sh
```

### 3. update cronjob


```bash
$ crontab -e
```

#### append following line
``` 
* 2 * * * ~/bing-wallpaer/bing-wallpaper.sh
```
