---
layout: page
title: Serpens Eternal Thievery
subtitle : PC, Immersive First Person Stealth Game
---

<video width="100%" height="540" controls poster="/assets/img/Steam_MainCapsuleV3.png">
  <source src="/assets/img/Serpens_PortfolioTrailer.mp4" type="video/mp4">
</video>

### Summary
Serpens: Eternal Thievery is an immersive first-person stealth game where you embody Anika, a thief gifted with the power to loop back in time. With this unique ability and your arsenal of weapons, you must explore treacherous places, fight challenging enemies, and keep to the shadows.

### Role
I was lead programmer, artist and designer on Serpens: Eternal Thievery. I juggled all duties throughout a development time (for the Scree Abbey level) of about 8 months.

### Challenges
Development for Serpens: Eternal Thievery presented several challenges in all disciplines.

#### Programming

I needed to construct a solid and modular sensory system for NPCs in the game for sight, hearing, touch, and smell. This sensory system needed to feed into a many-behavioured AI decision maker (a hierarchical finite state machine). 

#### Art

Serpens: Eternal Thievery is a retro game visually inspired by the late 1990s and early 2000s games. Games of that era had reduced color depth and lower resolution. I wanted to keep those constraints but use some modern features like dynamic lighting and shadows to increase dynamism of stealth encounters. I had to modify the built-in shaders of Unity to tweak the lighting and its attenuation.

#### Design 

Reconciling a stealth game with a time loop mechanic is no easy feet. In such a game, infiltration needs to be much quicker than traditional stealth games because players will repeat the infiltration over and over again. Instead we want to make infiltration easier and instead add many ways of infiltrating so that each loop stays fresh. 

Another challenge is to keep players engaged and retain some intentionality at the start of each loop. Each part of the map needs to be populated with interesting encounters that redirect players towards the desired areas of interest.

A lot of work must also be done to make the dynamic nature of time interesting and understandable. In Serpens, time moves forward during the loop and NPCs change their behaviour as the loop progresses. This creates many issues as to guiding players towards AOI (areas of interest) because they might go somewhere at a certain time, see nothing, and assume this is the case for the entirety of the loop. We must thus leave crumbs for the players to find in areas where nothing currently happens, but something does. The entire level is an interconnected ecosystem. Characters travel in many areas around them, and killing some characters will have ripple effects on other occurences in the loop.  

### Learning Outcomes

<ul>
  <li>Understanding of HFSMs and crafting complex sensory systems that ramp up progressively.</li>
  <li>Better understanding of crafting game mechanics that feel good.</li>
  <li>Knowledge of designing stealth games and engaging levels.</li>
</ul>

### Tools

Unity 3D, C#, Maya, Blender, Wwise, HLSL

### As Seen On

<p align="center"><iframe src="https://store.steampowered.com/widget/2642850/" frameborder="0" width="80%" height="190"></iframe></p>

<p align="center"><blockquote class="twitter-tweet"><p lang="en" dir="ltr">A small gameplay trailer for Serpens&#39;s Steam page <a href="https://t.co/2PWAM08Pgo">pic.twitter.com/2PWAM08Pgo</a></p>&mdash; Thomas Porta (@TPTP_dev) <a href="https://twitter.com/TPTP_dev/status/1714698313788707026?ref_src=twsrc%5Etfw">October 18, 2023</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></p>

### Alpha Gameplay

<p align="center">
<iframe
    frameborder="0"
    width="80%"
    height="270"
    src="https://www.youtube.com/embed/6OOhyQ7Vap8?mute=1"
    allowfullscreen
> </iframe></p>

### Additional Screenshots

![Serpens1](/assets/img/gamEnv1.png) <br/>

![Serpens2](/assets/img/gameSneak2.png) <br/>

![Sirenum3](/assets/img/gameCombat2.png) <br/>

![Serpens4](/assets/img/gameEnv3.png) <br/>



