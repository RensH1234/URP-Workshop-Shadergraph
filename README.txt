README

This part of the workshop will be about the shadergraph. We'll learn about some basic parts of the shadergraph editor and how to use nodes.
Also, we'll see if you can make something cool with shadergraph.

When you open the project you should see 3 rectangles. 1 has a material with mossy rock texture. This is a normal material with just a base map to show the texture. It looks fine, but the texture is reusable everywhere else. What if I want a more green version of the texture?
I can change the base color. But what if I just want the green part to be greener?

You're gonna make a shadergraph for a material where you have an input for the base map, the texture, and an input field where you set how green the green has to be. To start, go to Assets > Materials and create a new Shadergraph. It should be an URP Lit shadergraph. Open it.

You don't have to understand everything you see in the shadergraph.
You'll see blackboard. In the blackboard, add a Texture2D called Base Map, and a Float called Green Factor. Drag them onto the board.

Select the base map and click on the graph inspector. set the default value to "MossyRock". This makes it easier to work with. Set the default value of green factor to 1.

To start, click on the black dot on the base map and connect it to a "Sample Texture 2D" node. Now that in the end, your final image has to go to "Base Color". Tip: Use multiply and vector3 nodes.

If done, try to make a shadergraph that can blend multiple textures together (use the blend node).