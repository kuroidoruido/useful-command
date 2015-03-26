# Videos

##### concat videos
```
mencoder -oac copy -ovc copy -idx -o out.mp4 int1.mp4 in2.mp4 in3.mp4
```

##### reduce duration / fast playback / reduce frame number (divide by 2 = 0.5*)
```
ffmpeg -i in.mp4 -filter:v "setpts=0.5*PTS" out.mp4
```
