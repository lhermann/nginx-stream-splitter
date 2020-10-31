# Nginx Stream Splitter

Designed to split a OBS stream and re-stream it to multiple youtube live streams

## Setup

```
docker-compose up
```

## Test it

Stream a video from your computer with this command:

`ffmpeg -stream_loop -1 -re -i 1080p-THX-genesis.mp4 -f flv rtmp://localhost/restream`


