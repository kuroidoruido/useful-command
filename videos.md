# Videos

##### concat videos
```
mencoder -oac copy -ovc copy -idx -o out.mp4 int1.mp4 in2.mp4 in3.mp4
```

##### reduce duration / fast playback / reduce frame number (divide by 2 = 0.5*)
```
ffmpeg -i in.mp4 -filter:v "setpts=0.5*PTS" out.mp4
```

##### extract all images from a video
```
ffmpeg -i in.mp4 -r 1 -f image2 image-%3d.png
```

##### screencast
```
ffmpeg -f x11grab -r 25 -s 1366x768 -i :0.0 -vcodec huffyuv screencast.avi
```
