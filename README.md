# cle
Command Line Essentials
## cmatrix
### Having fun on the console, rainbow matrix screensaver
```
cmatrix -abr
```
## convert
### Create animated gif from multiple images and loop forever
```
convert -loop 0 -delay 200 1.png 2.png 3.png 4.png 5.png 6.png 7.png 8.png output.gif
```
---
## [ctop](https://github.com/bcicen/ctop) - top-like interface for docker container
```
ctop -a
```
---
## curl
### Receive public IP address
```
curl ifconfig.me/ip
```
---
## diskutil
### Erasing sd card and formattig with FAT32
```
sudo diskutil eraseDisk FAT32 SDCARD MBRFormat /dev/disk2
```
---
## docker
### Build image from Dockerfile with tagging
```
docker build -f Dockerfile -t flow1985/openttd-jgr .
```
### Run command inside container
```
docker exec -it b9edef51a553 /bin/bash
```
### Show logs from container
```
docker logs -f b9e
```
### Run container with port forwarding and volume mounting
```
docker run -d -p 8080:8080 -p 8081:8081 -v /Users/florianwallburg/Documents/MyProject:/usr/src/app sapui5-ide-docker:1.69.0-sdk
```
---
## dwebp
### Decode webp format
```
dwebp input.webp -o output.png
```
---
## ffmpeg
### Convert video to x264 and copying video and audio
```
ffmpeg -i file.mkv -c:v libx264 -c:a copy -c:s copy -n out.mkv
```
### Concat videos from list.txt to one single file
```
ffmpeg -f concat -i list.txt -c copy 20250510.MOV
```
### Concat videos from list.txt to one single file w/o audio
```
ffmpeg -f concat -i list.txt -c copy -an 20250510.MOV
```
### Concat videos from list.txt to one single file w/o audio and send it to background processing
```
nohup ffmpeg  -nostdin -f concat -i list.txt -c copy -an 20250510.MOV &
```
### Speed up video by 10 times
```
ffmpeg -i 20240510.MOV -an -vf "setpts=PTS/10" 20240510_10x.mp4
```
### Speed up video by 10 times and resize to 640x480
```
ffmpeg -i 20240510.MOV  -vf "setpts=PTS/10, scale=640:480" -an 20240510_10x.mp4
```
---
## find
### Copy only files from directory and subdirectories to current folder
```
find . -type f -exec cp {} . \;
```
---
## gifify
### Creates animated gif from image files
```
gifify -p 800:577 -r 1@1 -o my-gif *.png
```
## git
### Presents the list of commits with hash one per line
```
git log --pretty=oneline
```
---
## history
### Grep a certain command from history
```
history | grep docker
```
---
## homebrew
### Install brew formula
```
brew install gifify
```
---
## ncdu - NCurses disk usage
### Analyzing disk usage
```
ncdu
```
---
## nmap - the Network Mapper
### Scan a network and find out which servers and devices are up and running
```
nmap -sP 192.168.1.0/24
```
---
## npm - node.js package manager
### Install without dependencies in package.json
```
npm install --production
```
---
## python
### Serve current directory tree at http://$hostname:8000
```
python -m SimpleHTTPServer
```
## sed - stream editor
### Search and replace text inside a file
### Remove specific line from file specified by line number
```
sed -i '76d' src/rev.cpp.in
```
---
## sox - audio interface
### Merge all *.mp3 after one another into one single .mp3 file while using bitrate 192kb/s 
```
sox 0*.mp3 -C 192.01 -c 2 -S "Benjamin Blümchen - 026 - Als Bademeister.mp3"
```
### Take the first 120 minutes from a audio file
```
sox jAOW8-u1Xh8.mp3 output.mp3 trim 0 120:00
```
---
## sudo - 
### Execute previous command with sudo
```
sudo !!
```
---
## tar with gzip - tape archiver :) and gunzip
### Create .tar.gz with highest compression
```
env GZIP=-9 tar cvzf file.tar.gz /path/to/directory
```
### List the content of a .tar.gz file
```
tar -ztvf file.tar.gz
```
## tmux - terminal multiplexer
## tmux - terminal multiplexer
### Create new session
```
tmux
tmux new
```
### Resume old session (attach)
```
tmux a
```
### Close current session (detach)
```
Prefix + d
``` 
## yt-dlp - youtube download client for command line
### Show all donwload formats
```
yt-dlp -F https://www.youtube.com/watch\?v\=1__CAdTJ5JU
``` 
### Download audio source from video as mp3
```
yt-dlp -f 140 -x --audio-format mp3  https://www.youtube.com/watch\?v\=1__CAdTJ5JU
``` 




