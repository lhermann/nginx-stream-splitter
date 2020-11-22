# Nginx Stream Splitter

Designed to split a OBS stream and re-stream it to multiple youtube live streams

## Setup

1. Clone this respository
2. `cp nginx.example.conf nginx.conf`
3. Edit `nginx.conf` and edit/add as many `push` directives as you want
4. Run the container `docker-compose up` (or in the background with `docker-compose up -d`)

## Documentation

Thos article describes the setup and usage in detail: https://lukashermann.dev/writing/splitting-an-obs-stream-to-multiple-destinations/

## Test it

Stream a video from your computer with this command:

`ffmpeg -stream_loop -1 -re -i 1080p-sync-test.mp4 -f flv rtmp://localhost/restream`

_Test video credits: https://www.youtube.com/watch?v=ucZl6vQ_8Uo_


