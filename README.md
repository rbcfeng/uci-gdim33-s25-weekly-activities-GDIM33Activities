# GDIM 33 In-Class Activities
## W1
### Activity 1
[Inspiration Board](https://miro.com/app/board/uXjVGoFY_sQ=/?share_link_id=458748029062)

1. A lot of the images on my inspiration board are pretty cohesive, since most of the images includes blue hues. The most common aesthetics of my images include frutiger aero and cybercore aesthetics. The game will be placed in a city setting with aquatic elements like water drops and sea creatures. There will also be tech elements, like old phones and other retro technology from the 2000's.
2. One of my table mates likes Elden Ring's landscapes and fantasy combat fight scenes. We both share a similar color scheme of bright colors.
3. The LA and I both share a taste in random games. We have played Fortnite and Minecraft before and we don't really have a very specific taste in games.


### Activity 2
<img width="960" height="720" alt="Break-down Week 1 Activity 2 (1)" src="https://github.com/user-attachments/assets/39d62e0f-5483-4ac5-8ec9-a8a44534ed89" />



## W3
### Activity 1
<img width="987" height="738" alt="Screenshot 2026-04-15 175410" src="https://github.com/user-attachments/assets/8fe75a13-c7cf-4d3a-854b-b5960613630a" />


### Activity 2
1. It is advantageous to save the event name for the explore-to-dialogue state transition as Scene variable because this transition will have to control the animals' fall, the cursor lock of the player, and the dialogue of the walrus. Saving it as a Scene variable will allow the affected objects to function properly without having to reference all the time, like a Singleton.
2. The Debug.Log() node allowed me to check if the transition from the exploration state to the dialogue state works. I was testing if the transition works, but I noticed that the debug message did not pop up on the console when I ran the game. I checked my graph and it seems that I've used the wrong node for the mouse click on the walrus. Because of this, I noticed that I've used a custom event, rather than the OnMouseDown node for the mouse click. From this, I was able to get the transition from exploration to dialogue to work.
3. The SetCursor Lock state will probably not be relevant to my Vertical Slice, because it is a 2D visual novel game, so the player will have to explore the background by clicking on UI and dialogue options.
4. The concept of "game state" will be relevant to my Vertical Slice because there will be a exploration state and a dialogue state. The exploration state will display the quest UI, as well as UI for the amount of money the player has and the time remaining. The dialogue state will include the sprites of the NPC and the player, as well as the dialogue and option buttons.



## W4
### Activity 1
In my build, the only thing that is playable right now is advancing the dialogue and choosing the player replies. My playtesting goals include how much the writing makes sense and if the dialogue UI is easy to understand.

Playtest Team: Sebastian Magana, Landon Her, Rebecca Feng, Kaleb Reyes, Jess Tran, Frances Kim

Playtest Notes:
- The UI buttons are a little pixelated. Change the settings to point.
- The pause between the end of the dialogue and the player replies appearing is a little too long. Consider shortening removing the waiting seconds.
- Think about where the click to interact will align.


### Activity 2
1. A writer could add more dialogue because they would only be editing the Scriptable Objects, then adding it onto an array which will be handled by the NewDialogueEvent Node. Buttons for the player's replies will also automatically be added because they would be instantiated.
2. The limit would be the dialogue nodes that fill may fill up the screen, otherwise the number of dialogue nodes are limitless.
3. Regenerate Nodes will update the nodes that are written in code to be created in the Script Graphs to use.



## W5
### Activity 1
ScriptableObjects - Branching Dialogue Quest System
1. When interacting with the NPC Boss character after the first conversation, there is an if statement in the NPC Boss scripting graph that checks if the correct item has been choosen. Test if the if statement functions properly through a debug log message that returns the output of the if statement.
2. Create one ScriptableObject for a quest state for giving the correct item if the if statement returns true, then the quest state will return a positive outcome. In the console, the debug log message should display a positive message for giving the correct item, and the message that the sprite is updated.
3. In the UI, the dialogue box and the dialogue text should show up, along with a cheerful sprite of the NPC Boss, but the text will not be updated. Test this by running the game.
4. In the NPC Boss scripting graph, use the Set Text node to get the dialogue text and have the input be the ScriptableObject successful quest state that updates the text with the string list in the ScriptableObject that displays first index of the positive messages. Test this by running the game.
5. Use a for each loop that reads each element of the string list in the successful quest state ScriptableObject upon player mouse click. The messages should appear in the Debug Log. Test this by running the game.
6. Use a Set Text node to connect the for each loop to update the positive messages on the dialogue text for each player mouse click. Test this by running the game.
7. Create a custom event and a variable that represents how much money the player has. The custom event is triggered when the dialogue of getting the correct object ends. Test this by creating a debug log message that indicates that the money reward event is triggered.
8. Create a quest HUD that displays the amount of money the player has in a textbox. Hook up the text with the triggered custom event by connecting it with the Set Text node. Test this by running the game.


### Activity 2
I was able to build the feature of collecting the phone, as well as displaying the positive messages when the player collects the phone in the debug log before class ended.



## W6
### Activity 1

1. Something that is new in the playtesting build from Milestone 1 is how the player can now collect a phone item and complete the NPC Boss's quest. There is dialogue implemented that shows the NPC's reaction to completing the quest.

2. [Itch Link](https://rebeccf2.itch.io/playtest-2-for-milestone-2)

3. Playtesting goal: My playtesting goal is for the playtesters to find any bugs that are present, aside from the ones I have already found in the build.

Playtesting Notes:
- Clicking the phone item to complete the quest is intuitive
- No UI is needed to tell the player to interact with items if they already know that they can interact with the NPC by clicking on it


### Activity 2
1. The Multiply setting makes the resulting color darker and less saturated because when the RGB values are mulitplied with two colors, their values from 0.0 to 1.0 will decrease since it would be multipled by numbers 1 or less than 1. As the values decrease, the color will be darker and less saturated.
2. The resulting value will be more translucent because as the alpha value is multipled that is 1 or less than 1 to the RGB value, the resulting value will decrease, which means the value is approaching towards 0, which means more transparency on the 0.0 to 1.0 alpha value scale.
3. The shader gets the UV values from the UV map of the shiba material.
4. This sounds exciting to me because although I may not be the best at math, learning about how blending colors work will be very useful when I draw digitally using blending modes.



## W7
### Activity 1
1. The data from the Vertex color node came from the color vertex data of the shiba mesh.
2. The color on the shiba is blended at the edge of different regions of color because each vertex of the shiba mesh creates interpolation, which blends the colors from each vertex depending on the distance between each vertex.
3. The shiba from step 3 is less detailed than the shiba from last week because the vertex color is used to check errors of the mesh data, rather than be something that will be displayed in game. The vertex color can be used to check for errors when breakpoints of Debug Log nodes are unable to check for them.
4. There is an error of vertex normals in a small area near the shiba's tail above the hind legs on the left. There appears to be a small dent in the mesh.
5. We can use the color output of a shader to determine the UV vertex data and test if the textures are consistent with the mesh, and that it maps correctly around the model.
6. There is an error in lighting on step 4 because the vertex normals are not consistent with the surrounding areas. There is a dent, rather than a consistent smooth surface of the shiba model.
7. The Blend Mode is set to Additive because it allows the colors to appear brighter, while the darker colors of the texture stays the same color.



## W8
### Activity 1
1. Something new in my build since Milestone 2 is how the player is able to change Scenes to another place in the office.
2. [Itch Link](https://rebeccf2.itch.io/milestone-2)
3. Playtesting goal: My playtesting goal is for the playtesters to give insight on the UI of the scene.

Playtesting Notes:
- There should be a price UI that shows how much the retro game console costs, so players aren't skeptical about what the purchase button does.
- The phone item should be in another room so they don't click on it first before they talk to the NPC boss for initiating the quest.

### Activity 2A
1. We are utilizing the stencil buffer in that the Compare Function is used to determine the pass/fail operations of values of the shiba object. The stencil buffer acts like a "stencil" in that for each value, depending on where it is on the Scene. If the outline is on the shiba object, then the shiba color buffer will be drawn and replaces the outline value when the value passes. As a result, this creates the effect of the outline of the object.
2. The DrawOpaqueObjects rendering pass seems to be drawing almost the exact same thing twice. It is being drawn twice because it is using two different shaders, one for the ground and one for the shiba in the Scene. The ground is using the Universal Rendering Pipeline Lit shader, while the shiba object is using the Cel Shading shader.
3. To improve this inefficiency, it might be a good idea to have both the objects use the same shader. The ground could also use a Cel Shading shader, or the shiba object could use the Universal Rendering Pipeline Lit shader.
4. The range of values from -1 to 1 for DarkShadowsAmount makes sense because the values are like a percentage, like 0.9 represents 90% and 1 represents 100%. The negative values represent the reverse of shadows and light, like how shadows on an objects swaps where the light is casted on the object.
5. We added instead of multiplied the results of all the different lighting because when the results are multipled, they only darken the colors, rather than keeping the results light and visible.
6. Changing the Layer of where the Shiba is on enables and disables the outline because the Outline layer uses the stencil buffer and the Outline shader to achieve the outline effect, while the Default layer only uses the Cel Shading shader for the shiba. When the Outline layer is enabled, the outline effect is in play.
7. Setting the shadow color to white removes the lighting because since the shadow color is set to multiply on the Shader Graph, when the color is white, the colors do not get darker, and instead stays the same original color.


8. I think a performance implication might include avoiding to modify material settings on an Update event because the program might produce a lot of copies of a material every frame. It might be better to modify a material when a certain event happens instead.
