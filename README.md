# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Joseph DeMario

Time spent: 5 hours spent in total

Link to project: 
Live Site - https://sable-marvelous-sardine.glitch.me 
 Code - https://glitch.com/edit/#!/sable-marvelous-sardine

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [X] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [X] Player only loses after 3 mistakes (instead of on the first mistake)
* [X] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
![](your-link-here)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
https://www.w3schools.com/js/js_random.asp
https://www.w3schools.com/cssref/css_colors.asp
https://www.w3schools.com/cssref/pr_background-image.asp
https://javascript.plainenglish.io/how-to-generate-an-array-of-random-numbers-in-javascript-f883de667e84

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
One challenge I encountered in creating this submission was how to randomly generate a pattern at the beginning of the game.  At first, I tried to create a function 
called randomizePattern() to generate a random pattern.  In this function, I declared an array called pattern.  Then, I created a for loop that iterates 16 times 
(since the pattern I intended was 16 buttons long), initializing each index in the array pattern to a random number.  I used Math.random and Math.floor to make this 
possible.  Since there are 8 buttons in my game, I want an aray that contains numbers in between 1 and 8,  In order to do that, I used the statement 
Math.floor(Math.random() * 8) + 1, which randomly generates a number between 1 and 8.  After the completion of this function, I called it in my startGame() function.
However, when I went to play the game, a randomized pattern failed to generate.  After coutless trial and errors, I was able to work around the problem.  Instead of 
creating an entire function to randomize the pattern, I placed the entire implementation where the global variables were placed.  In doing so, I knew for certain that
a randomized pattern was being generated before the startGame() function was called.  After multiple game attempts, I was able to tell that a randomized pattern was 
generated every time I played.   

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
Some questions I have about web development after completing my submission involve how to make a web application more visually appealing.  For example, how would I 
craft a website that contains animations, where as the user scrolls down the page, elements slowly transition onto the page.  I would also like to know how to animate
an element on the page when hovering over it.  Furthermore, I am also curious as to how to implement user authentication (register/log-in/log-out) from the back-end
and be able to connect it to the front-end of the web application.  Lastly, how would you be able to implement payment methods (like paying for a Netflix 
subscription on their website) in order to profit off of your site?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I had a few more hours to work on this project, I would have liked to add more CSS to my web application to make the game more visually appealing.  I also would 
have liked to order the functions in a more meaningful way so other developers know exactly where to look if they want to add an additional feature to the web 
application.  In addition, I believe providing clear and concise comments to each function in my script.js file would make it easier to traverse the file and find out
where to change or add certain features.  Lastly, I would have liked to add audio clips that correspond to each button that is pressed instead of using high and low 
pitch sounds as well as add a ticking clock.     



## License

    Copyright Joseph DeMario

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
