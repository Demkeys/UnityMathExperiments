## Lissajous Curve ##
This script is meant to be used in the Unity Game Engine. This script calculates the position of this gameobject based on a Lissajous Curve formula. You can change the values for the various parameters of the formula to customize the curve. The gameobject should have a Trail Renderer attached to it, so that the trail shows the curve.
Read up on Lissajous Curve on Wikipedia to understand the formula, and to also understand the various ways you can control the curve.
Link: https://en.wikipedia.org/wiki/Lissajous_curve

Instructions:
* Create an empty gameobject or primitive gameobject (Cube, Sphere, etc.)
* Set the gameobject's scale to (0.1,0.1,0.1)
* Attach a Trail Renderer component to the gameobject.
* It is suggested to set following Trail Renderer fields:
  * Material = Any material you have created. This will let you set a color for the trail
  * Time = 1000 (Just to keep the trail alive for a long time)
  * Width = 0.02 (or something similar so the trail isn't too wide)
* Attach LissajousCurve.cs script to the gameobject and set whatever parameters you want. There are also checkboxes allowing you to make certain parameters random.
* Drag and drop the attached Trail Renderer component into the TR field of the 'LissajousCurve.cs' script.
* Disable the Trail Renderer component because the script will enable it when needed.
* Set values for A, B, C, D, Delta, TimeMultiplier and Multiplier. Alternatively you can leave them at default, or generate them randomly by clicking the relevant checkboxes.
* Once you're done setting values, enter Play Mode.

_NOTE: Each time you wanna change values, exit Play Mode. If you change the values during Play Mode, the design of whatever pattern is currently being drawn will get messed up._

![](https://github.com/Demkeys/UnityMathExperiments/blob/master/LissajousCurve/LissajousCurveScreenshot.png)
