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
