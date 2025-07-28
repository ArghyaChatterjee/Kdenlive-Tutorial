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

## How to add/overlay videos to run simultaneously?
Answer:

**1. Apply Crop Effect**
* Click on the clip in the timeline (either V1 or V2) that you want to crop.
* Open the **Effects** panel in **TimeLine** (`Ctrl+Shift+E`).
* Search for **Crop** (or **Crop, Scale & Transform** if you want everything in one).
* In the **Effect Controls** for that clip, you’ll see sliders or numeric fields for **Top**, **Bottom**, **Left**, and **Right**.
* Increase each value to “cut off” that much from the corresponding edge.
* You can scrub through the video in the Project Monitor to make sure you’re cropping exactly where you want.
* If you used the simple **Crop** effect, you can then add **Transform** (or **Scale & Transform**) afterward to resize or reposition.
* The order in the Effect Controls panel matters—effects at the top apply first. You can drag them to reorder.
* For your inset clip on **V2**, first crop out any unwanted borders (e.g. black bars or extra top padding).
* Then scale it down and move it into the corner as before.


**2. Apply Transform Effect**

* Select the clip on **V2**, then go to **Effects** from **Timeline** (press `Ctrl+Shift+E`).
* Search for and add **Transform** (or **Crop, Scale & Transform** in older versions).
* In the Effect Controls panel, under **Scale**, reduce the size to whatever percentage you want (e.g. 20–30%).
* Still in the same effect, adjust the **Position X** and **Position Y** sliders (or drag the clip’s bounding‑box handles directly in the Project Monitor) so that the scaled clip sits in the lower‑left or lower‑right corner.
* Play back in the Project Monitor to make sure both clips run in sync.
* Trim or stretch clips on the timeline if you need to adjust their lengths.



