# HLS & DASH example

## Running this example locally

You can run this example locally with Docker runtime

```
% docker run -p 3030:80 -v $PWD/videos:/opt/static/videos -v $PWD/nginx.conf:/usr/local/nginx/conf/nginx.conf supermicro/nginx-vod-module
```

After running this command, you should be able to play the following URLs:

- HLS: http://localhost:3030/hls/sample,360p.mp4,480p.mp4,720p.mp4,.en_US.vtt,.urlset/master.m3u8
- Dash: http://localhost:3030/dash/sample,360p.mp4,480p.mp4,720p.mp4,.en_US.vtt,.urlset/manifest.mpd
- Thumbnail: http://localhost:3030/thumb/sample360p.mp4/thumb-1000.jpg
