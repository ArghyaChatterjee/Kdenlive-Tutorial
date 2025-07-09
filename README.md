# All About Kdenlive
This repository is for creating a tutorial about video editing with Kdenlive and some tips and tricks about video editing.

## How to perform crop on a video in Kdenlive ?
Answer:

There are 2 ways to perform crop.

1. To apply the Crop Effect, click on the video clip in the Timeline to select it.
   - Go to `Effects` tab on the top right panel.
   - In the search bar under the Effects tab, type “Crop”.
   - Drag the `Crop (Center)` effect or simply `Crop` (depending on your version of Kdenlive) onto your video clip in the Timeline.

2. With the video clip selected in the Timeline, go to the `Effect Stack` tab --> `Transform, Distort and Perspective` which is also on the right panel.
   - You will see the Crop effect listed there. Click on it and go to `crop by padding`.
   - Adjust the `Left`, `Right`, `Top`, and `Bottom` values to control how much of each edge to crop. The adjustments can be made using the sliders or by entering values manually to get precise control.

## How to convert an mp4 file, cropping to a certain resolution?
Answer:
If the cropping amount for the width is 220, and for the height is 42: 
```
ffmpeg -i input.mp4 -filter:v "crop=1700:1038:110:21" -c:a copy output.mp4
```
You can also get the output file in `gif` format.

## How to convert an MP4 file to a GIF file ?
Answer:

Once you generated the mp4 file from the Kdenlive render, use command line tool:
```bash
ffmpeg -i input.mp4 -vf "fps=5,scale=640:-1:flags=lanczos" -c:v gif output.gif
```
