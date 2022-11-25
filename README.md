# Video streaming CDN with varnish

## Run

```
$ docker-compose up -d
```

## Prepare content

Put a mp4 file into `storeage/site-content/video`

```
ffmpeg -i input.mp4 -g 60 -hls_time 2 -hls_list_size 0 out.m3u8
```

## Test streaming

Visit `https://www.hlsplayer.net/` and next url:

`http://localhost:9000/video/output_1080.m3u8`
