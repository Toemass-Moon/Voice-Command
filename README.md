# Voice Command
#### Thomaz Moon

---
## Problem Statement
There are times when you're in a comfortable position and want to do something on your computer without having to move just quiet yet. Or you're a bit too busy to type or move the mouse at the moment. This project will tackle the idea of having a voice command assistant that can do certain tasks simply by telling your computer what to do. Similar to a "okay google" or "Alexa".

## Executive Summary
We all know the usefulness of voice activated virtual assistants such as an amazon echo or google home. Both devices however won't help you much when you're on your computer. In this project, we will code out a voice command that can do a variety of things on your computer, such as:

| Regarding the Browser | General Tasks |
|---	|---	|
| Open a website on the current or new tab 	| Raise or Lower the volume by said amount 	|
| Minimize or Maximize the window 	| Take a screenshot 	|
| Close the current or last tab 	| Open League of Legends 	|

**Here is a gif demonstration. Although you can't hear anything, on bottom right hand corner you will see `Talk now` whenever I say the word "computer"**
<img src = './notebook_imgs/voice-control-gif.gif'>  

## Basic Structure
1. The 1st notebook `01 Messing Around` is simply where I found how many more pixels I wanted to move my mouse in order to get to the desired location. When I take a screenshot of the items I want found, such as the `X` or "minimize" button, the original position will take my mouse to the edge or the image, however, by adding in a few more pixels, I can get to the center of the image where I actually want to click.  

> <img src = './notebook_imgs/new_tab.png' align> **for example will require me to move an additional 7 pixels to the right and 15 pixels down like so** <img src = './notebook_imgs/moving_example.png'>

2. The 2nd notebook `02 Voice Command` is where everything is put together. We use `speech_recognition` along with `googles voice recognition api` in order to translate spoken words to text.  
There are a lot of elif statements for all the different possibilities that can be said, as well as a "Turn off" command to prompt the loop to break and stop, so the code looks a bit long, but everything can be broken down and easily understood in conjunction to the first notebook in case anything is confusing.

## Next Steps
Some next steps or possibilities could be to add in more features sure as "What's the weather like" or "directions to _____". This project is just more of an overview of **how** to get the voice recognition working together with pyautogui. Some parts are a bit crude as well such as using the word `open (website)` in order to make a new tab, however I only check for the word `open` to make a new tab. Adding in some more measures in order to be able to use the word `open` on other things would easily be doable. 
