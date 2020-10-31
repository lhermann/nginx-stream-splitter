# Nginx Stream Splitter

Designed to split a OBS stream and re-stream it to multiple youtube live streams

## Setup

1. Clone this respository
2. `cp nginx.example.conf nginx.conf`
3. Edit `nginx.conf` and edit/add as many `push` directives as you want
4. Run the container `docker-compose up` (or in the background with `docker-compose up -d`)

## Test it

Stream a video from your computer with this command:

`ffmpeg -stream_loop -1 -re -i 1080p-sync-test.mp4 -f flv rtmp://localhost/restream`

_Video source: https://www.youtube.com/watch?v=ucZl6vQ_8Uo_


