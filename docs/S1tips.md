# Scenario 1 specific tips
This guide is for early testing participants who are less familar with Unity and would like to understand topics related to the first session

## How to Animate

For animating your character in Unity you will be using the animator component 
To see the animator for the player make sure you're currently selected on the player object in the scene view.

Then go to Window/Animation/Animator in the top menu bar
It is **not recommended** to touch the animator graph as it's already been setup for you. You just need to use code to make it work which is very simple.
![Alt Text](Images/Animator.png)

I recommend watching this video to learn how to play your own animation.
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/tveRasxUabo?si=_RO4H9d609BIpuKx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For clarification **Jump** and **Land** are triggers but **Walking** is a bool value. (hence why it's a square) You won't need to use the walking value for this demonstration. 

![Alt Text](Images/AnimatorValues.png)
