# Portfolio



## Week: 1
The first week of this semester was very similar to the first week of last semester. However, this time I did not have to choose which project I was doing as I had signed up to continue working on the Game Development project. This time I knew I was working on the big game instead of just a smaller side project. I met up with my team for this semester, and it was just me and Mitchell, who I had been working with partially last semester. We set up our workspaces and got a debrief of what this game was all about. This game really interested me, and I was excited to begin working on it.

### Reflection:

## Week: 2
The second week presented our first set of problems. We didn't have any up to date versions of the game from last semester. We had the files that were stored on GitLab, but they did not include all of the assets due to them being too large to go onto GitLab. Our project leader, Adon, said that the previous students to work on this project had stored their assets onto a server. This presented another problem. We had no access to the servers as the keys had expired to use the servers, so we had to wait until the dev-ops team could get them back into our posession.

### Reflection:


## Week: 3
This week finally allowed us to start work on the project. We managed to get a copy of the up to date version of the game. This week was primarily about learning how the game worked. Much of this stuff was new to us both, and we had to learn a lot before diving into this, as we both had not worked on a multiplayer game before. I was also assigned my first task. I was to make a Heads Up Display (HUD) for the user's that displayed their health, their posession timer and a third undecided bar (perhaps a stamina bar). We had some assets from the design school, so I just had to program them to be linked into our player's health and posession values, then animate the images. I got this working well locally, however I tested it on a server side and the local player's HUD controlled all clients who connected to the server's HUD. This was something I needed to fix next week.

### Reflection:


## Week: 4
My first task of the week was to finish this HUD, as Adon really wanted it out of the way. I figured out that to fix this problem I was having, was that I needed to have each component of the HUD to be displayed on each player's individual cameras. This took a wee bit of thinking, but in the end it was a rather easy solution, and I got it up and running pretty quickly. I believe at this point, Adon decided that I was going to be doing the design side of the game primarily, as the next task I was assigned was to make a pause menu for the game. Luckily, this ended up being an almost identical process to the HUD, so I managed to get that done very quickly. This gave me some time to give these User Interfaces (UI) a good code cleanup. I gave them all dynamic methods, so that it was super easy in the future to add to these, and have them work in the network. 

### Reflection:


## Week: 5
This week, I finished the pause menu by having all of the pause buttons do something. Currently, we have no settings menu, so the settings menu just unpauses the game, but that's an easy fix. I also added in the SKIN font. Just to top things off, I added a nice slide in animation for the pause menu to make it look a little more polished. Adon was not here to give any more things to do, and I had already finished everything he wanted done, plus a few extra bug fixes, so I decided to get started on an inventory system. I created a temporary circle menu, similar to that from other survival games, and got all the base code setup for that.

### Reflection:


## Week: 6
I finished up the circle menu, by having all 4 slots working, and having it work properly on the network. This process was slightly different to the HUD stuff, as it also had to stop the local player's mouse movement while in it. Adon also told me to look into a demo designed by Unity called Book of the Dead. It was a demo showcase to show off the power of Unity, and contained a very beautiful scene. Adon wanted me to see if I was able to use some of their free assets to recreate the graphics shown off in this demo. I was told that the previous students working on this project couldn't get it to work, however I was optimistic. I learnt that this demo was running in a different rendering pipeline than the one our game was running in. It was running in the High Definition Render Pipeline (HDRP), which was very different to what we were using, and handled everything very differently to how our game currently handles stuff. Adon really wanted to get these assets working, and so did I, so I did my research on HDRP and learnt that I would need to create a whole new scene, and essentially rebuild the game from the ground up in HDRP. I created a new HRDP project, and put it aside until next week.

### Reflection:


## Week: 7
This week, we met with a design student who had been creating us a new Wolf asset for his design project. He sent us the files, and I decided to try and get this wolf working in both our original scene and the Book of the Dead scene. He came in the same day so I was able to learn which wolf he wanted us to use (as he gave us many different versions of it). We played around and got it working in our original game scene, and our original wolf AI eventually worked with a few tweaks. After we got all this working, I decided to try and get it to work in the Book of the Dead scene. I played around with the wolf's shaders, and eventually figured out how to convert it to an HDRP asset. This was crucial to figuring out how to implement more Book of the Dead stuff. The wolf now worked in the Book of the Dead scene, so I knew that next week I had something to work on. However, before that, I was instructed to create an intro scene for the game which included the Polytech's game studio logo (Forth Street Studio), as well as the SKIN logo, and a main menu. I setup a basic intro scene, which included some music that a music student created for us. I played around with timings and animations to get a basic intro scene that was in time with the music we were provided.

### Reflection:


## Week: 8
This week I began adding some particles to the intro scene. I suggested that we could have some smoke or something in the intro scene to make the black background a little more interesting, and he suggested I try and get a dusty/pollen looking particle effect to fit the theme of the game. I found Unity's own particle pack, which I took apart and grabbed their dust particle effects. I applied this to the intro and tweaked it a little and it actually looked pretty good. So I finished off this intro for now, and fixed up a new graphical features of the HUD, including an issue where the HUD started hiding behind certain objects in the scene. This just required me to apply a new shader to their UI. Once I got all of this working, I was able to get back to playing around with Book of the Dead. I played around with bringing assets between the two projects, but I was only able to bring assets from our game project into the Book of the Dead scene, and not vice versa. This meant that I would have to follow through with rebuilding the game in a new HDRP scene. Mitchell had recently built a temporary test terrain, which I was able to convert to HDRP and then bring into this new scene. From here I was able to get all of our old important assets to work in HDRP, and start creating a basic scene out of it.

### Reflection:


## Week 9:
An HDRP scene that contains Book of the Dead assets has been created! It was actually possible, after all of our struggles, I eventually got it working. I had only brought in a single tree and a single grass asset and built a very basic scene out of it. It didn't look anywhere near as good as Book of the Dead, so I decided to break down the Book of the Dead scene, asset by asset. I learnt that it uses some pretty intense post processing, which I was able to replicate similarily in our game scene which improved our visuals by a lot. I also learnt that the most important feature that Book of the Dead uses to make their scene to pretty, is a thing called Occlussion Probes. This is something that was custom built by Unity just for this showcase demo, and was far too advanced for 3rd year students, so unfortunatley, no matter how hard I tried, I wouldn't be able to make our scene as pretty as Book of the Dead. But that wasm't a bad thing, as I had now unlocked the secret to getting the 4K textured assets from Book of the Dead. Next step is to implement some more things into our game.

### Reflection:


## Week 10:
This was the last week of the term, so I wanted to just clean this game up and get it looking all pretty before the holidays so that I wouldn't need to worry about this stuff as much next term. I finished implementing some post processing, similar to what Book of the Dead uses, and honestly the game looks quite nice. It still has a lot to go before it is in a beautiful state, but I managed to get some nice lighting, shadows and details going in our scene. I brought some more assets from Book of the Dead into our new HDRP game project, and got them all working in here. I also needed to create a new sky for our scene. This is due to using HDRP, our old sky no longer worked, so I had to figure out how to make a HDRP sky. There were 3 options for this, however I just stuck with the basic HDRP sky for now as there is no need for anything more advanced.

### Reflection:


## Holidays:


### Reflection:


## Week 11:



### Reflection:

## Week 12:



### Reflection:


## Week 13:


### Reflection:


## Week 14:


### Weekend:


### Reflection:


## Week 15:



### Reflection:


## Week 16:



## Overall Reflection:
