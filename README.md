# Kdenlive Tutorial
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
  
## How to perform scaling on the video to fit the canvas in Kdenlive ?
Answer:

* Select the clip on **V1**, then go to **Effects** from **Timeline** (press `Ctrl+Shift+E`).
* Search for and add **Add Effect** --> **Transform, Distort & Perspective** --> **Transform**.
* In the Effect Controls panel, increase the **Size** to scale the size to whatever percentage you want (e.g. 120–130%).
* Still in the same effect, adjust the **Position X** and **Position Y** sliders (or drag the clip’s bounding‑box handles directly in the Project Monitor) so that the scaled clip fits the whole canvas.
* Trim or stretch clips on the timeline if you need to adjust their lengths.

## How to perform crop on a video and scale the video to fit the canvas in Kdenlive ?
Answer:

* First go to **projects** --> **project Setttings** --> select the resolution and fps for the project (default 1080p at 30hz).
* Select the clip on **V1**, then go to **Effects** from **Timeline** (press `Ctrl+Shift+E`).
* Search for and add **Add Effect** --> **Transform, Distort & Perspective** --> **Crop by Padding**.
* In the Effect Controls panel, always **Scale** first and do the other operations later. Scale to increase the size to whatever percentage you want (e.g. 120–130%).
* Still in the same effect, adjust the **Position X** and **Position Y** sliders (or drag the clip’s bounding‑box handles directly in the Project Monitor) so that the scaled clip fits the whole canvas.
* Trim or stretch clips on the timeline if you need to adjust their lengths.

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

## How to Face Blur in Kdenlive ?
Answer:

Go through this tutorial: https://www.youtube.com/watch?v=sFkJIzPglko

In **Kdenlive**, there are two common ways to blur a face.

**Method 1: Motion Tracker + Blur (Recommended)**

This is the easiest if the face moves.

* Import your video and drag it to the timeline.
* Select the clip.
* Go to **Effects** and add **Motion Tracker** (or **Motion Tracker (Face)** if your version has it).
* In the Motion Tracker effect:

   * Draw a rectangle around the face.
   * Click **Analyze** or **Track Forward**.
   * Let Kdenlive generate the tracking data.
* Add a **Blur** effect:

   * Search for **Gaussian Blur**, **Box Blur**, or **Pixelize** (pixelization is often better for anonymization).
* In the blur effect, choose **Apply to: Tracked Region** (or link it to the motion tracker, depending on your Kdenlive version).
* Adjust:

   * Blur strength or pixel size.
   * Region size so it fully covers the face.

The blur will automatically follow the face.

**Method 2: Manual Mask + Blur**

If the face doesn't move much:

* Add a **Blur** or **Pixelize** effect.
* Enable the effect's **mask/shape** (ellipse or rectangle).
* Position it over the face.
* If the face moves:

   * Move the playhead.
   * Click the **keyframe** button.
   * Reposition the mask.
   * Repeat every few seconds or whenever the face changes direction.

Kdenlive interpolates between keyframes automatically.





