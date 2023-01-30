---
layout: page
title: Technical Art
---

### Sirenum

Sirenum required a post processing effect to draw the outlines and apply a small amount of dithering. In order to draw the outlines I used a common outlining technique which detects discontinuities in the image rendered by the engine. Usually it is used with three sources of discontinuities - colors, normals and depth. You can find a good resource on this method [here](https://alexanderameye.github.io/notes/edge-detection-outlines/). In Sirenum I only use discontinuities in colors. I modelled all models and could manually set vertex colors where I wanted lines to appear. 

![Sirenum](/assets/img/Sirenum2.png)


### Moebius Style

After playing Sable, I set out in making a Moebius inspired graphic novel post processing shader. This also uses a discontinuity based outline detection algorithm but it uses all three sources of discontinuities. This is coupled with a simple binary lighting model. Either an object is lit with the color of the main light source or it is in shadows. I also allow objects to have an edge map texture for custom edges - this is done in another render pass. A bloom effect supplements all of the above to give objects an extra level of presence.

![Sable](/assets/img/Sable1.PNG)

### [Project Train](https://thomasporta.github.io/projecttrain/)

Project Train required a retro look and I did so through a post processing shader. This shader controls the allowed range of colors. While we mostly use the R8G8B8A8 format in modern engines, older engines had fewer bits per channel - 4 to be exact. This dramatically reduces the amount of colors you can create. (HDR uses more bits per channel, hence why HDR represents more colors, deeper blacks and better whites.) The shader controls how many bits are allowed for each channel, creating this old school feeling. We also control the rendering resolution to add pixelation. My work includes VFX for the game, one instance of which you can see below.

![ProjectTrain](/assets/img/PT1.png)

<video width="100%" height="540" controls poster="/assets/img/PT2.png">
  <source src="/assets/img/AlienVFX_comp.mp4" type="video/mp4">
</video>

### Gaussian Outlines

Gaussian Outlines are useful if we want soft outlines. They are built using a gaussian blur on select objects. Each object is rendered on a special render target and then blurred in two passes. One vertical and one horizontal pass. As such they can be expensive if used extensively. Despite this they are widespread. 

![GaussianOutlines](/assets/img/GaussianOutlines.PNG)

### Terrain Scanner

I created this terrain scanner to upload it for free on the Unity Asset store. There were not many alternatives and I thought it could be helpful to others. It has been downloaded several hundred times as of now. Good for prototyping and production. The scanner is a post processing effect and will work with any level geometry and materials, except transparent materials that do not write to the depth pass. The depth is used to reconstruct the world position of each pixel so that we can determine whether that pixel is within the range of the terrain scanner and whether it should me modified.  

<video width="100%" height="540" controls poster="/assets/img/StillTerrainScannerFP.PNG">
  <source src="/assets/img/TSV2_FP.mp4" type="video/mp4">
</video>
