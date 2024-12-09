# Intro to CG Final Exam
 
1+0+1+1 = 3 Prime

Shaders Implemented: Vertex Coloring, Outlining, Toon and Waves

Why I Implemented what I've implemented:

Vertex Coloring: more roads but different style

Outlining: Making the carts/players have a visible outline.

Toon: The game should look cartoony as Super Mario Kart is a cartoony game.

Waves: In rainbow road, the track goes up and down.

Rainbow Texture taken from here: https://www.google.com/search?q=rainbow+texture&rlz=1C1UEAD_enCA1011CA1011&oq=rainbow+texture&gs_lcrp=EgZjaHJvbWUqBwgAEAAYgAQyBwgAEAAYgAQyBwgBEAAYgAQyBwgCEAAYgAQyBwgDEAAYgAQyBwgEEAAYgAQyBwgFEAAYgAQyBwgGEAAYgAQyBwgHEAAYgAQyBwgIEC4YgAQyBwgJEAAYgATSAQgxMTk3ajBqN6gCALACAA&sourceid=chrome&ie=UTF-8#vhid=bnU9wN_FyfREhM&vssid=_Mi1XZ-HlKIDw0PEPvMzykQg_40

Normal Made with Photopea (photoshop alternative)

How I implemented everything:

Vertex Coloring:

There are no properties required because this is supposed to be a static shader that doesn't change. The shader looks at the object and finds all the vertices then applies the colors based on what was selected based on what vertices it can access. 

Outlining:

The properties are there because the shader needs to know the main texture, the color of the outline and the width of the outline. 
It takes into consideration of the direction that we look at it from and figures out where the vertices of the object are. 
When the vertices are found, everything is put together and then the outline is formed.

Toon:

The properties are there because the shader needs to know the main texture and color.
It takes into consideration of the direction that we're looking at the object from.
Applies toon by looking at lighting and darkness properties
Once everything is done, it puts the toon pattern on the character to give it the look that it comes from a cartoon show/game.

Waves:

The properties are there because the shader needs to know the main texture, color, scrolling properties such as how fast and how large the waves are.
Next in the subshader category, the program tells the system that I've made my selection on everything before, the program then realizes that this is the texture/material/normal that needs to be put on the object. The plane first starts off with realizing that it needs to move up and down to simulate the look of waves, then the image texture which would be my rainbow is moving from left to right and then the final look is formed.

![image](https://github.com/user-attachments/assets/05fd838d-a487-4b9b-ab4d-61d671ea4a45)
