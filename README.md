# AWS HLS Video Streaming using CloudFront + MediaConvert

This project demonstrates how to stream a video in multiple resolutions using HLS format via AWS CloudFront. Video was transcoded using AWS MediaConvert and hosted in a private S3 bucket, served securely via CloudFront.

## 📺 Master Playlist
```m3u
#EXTM3U
#EXT-X-STREAM-INF:BANDWIDTH=2000000,RESOLUTION=1280x720
https://d2a9nhafbib6xk.cloudfront.net/kannada/Movies/UDVEGA/720p/UDVEGA_720.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=4500000,RESOLUTION=1920x1080
https://d2a9nhafbib6xk.cloudfront.net/kannada/Movies/UDVEGA/1080p/UDVEGA_1080.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=8000000,RESOLUTION=2560x1440
https://d2a9nhafbib6xk.cloudfront.net/kannada/Movies/UDVEGA/2k/UDVEGA_2k.m3u8
#EXT-X-STREAM-INF:BANDWIDTH=15000000,RESOLUTION=3840x2160
https://d2a9nhafbib6xk.cloudfront.net/kannada/Movies/UDVEGA/4k/UDVEGA_4k.m3u8
