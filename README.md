# Pre-work - _Memory Game_

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program.

Submitted by: Shivasree Margam

Time spent: 4 hours spent in total

Link to project: https://glitch.com/edit/#!/beryl-judicious-empress

## Required Functionality

The following **required** functionality is complete:

- [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
- [x] "Start" button toggles between "Start" and "Stop" when clicked.
- [x] Game buttons each light up and play a sound when clicked.
- [x] Computer plays back sequence of clues including sound and visual cue for each button
- [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess.
- [x] User wins the game after guessing a complete pattern
- [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

- [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
- [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
- [ ] More than 4 functional game buttons
- [x] Playback speeds up on each turn
- [x] Computer picks a different pattern each time the game is played
- [x] Player only loses after 3 mistakes (instead of on the first mistake)
- [ ] Game button appearance change goes beyond color (e.g. add an image)
- [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
- [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
![reference](https://i.imgur.com/eMJHWfz.gif)


## Reflection Questions

1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.
*    I used stackoverflow a couple of times when I could not figure out how to change the playback speed.


---

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words)
*    One challenge I encountered in creating this project was trying to shorten the time after each sequence. clueHoldtime is what needed to be changed in order to be successful in developing this optional feature. First I changed clueHoldtime from a global constant to a global variable. The value of the clueHoldtime variable was set to 1000 value which was not changed. As noted in the project description, in order to add the feature, I tweaked the function playClueSequence. To decrease the time of the clue hold, I changed the clueHoldtime value in playClueSequence to clueHoldtime = clueHoldtime - 25; The value 25 took many tries to come up with since any number little less than 25 or little more than 25 affected the clue hold time significantly. Number less than 25 made the hold time seem unaffected and number above 25 made the clue hold time seem way too quick. Adding this feature raised a new error into the code. After the game ends, the clue hold time didn’t reset back to the original starting clue hold time. This meant that I had to set the value back to 1000 at the end of the game. I did this by setting the variable to 1000 if the user failed or passed the game in guess function.


---


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words)
*    One major question I have is whether it is possible to web develop with the use of only JS and CSS. In this project, there are multiple languages used such as HTML and Javascript. I was wondering if the same program can be implemented with the use of just two languages. Another question is whether using fewer programming languages would be faster than using many. Does using more than one increase the efficiency and time to create a project. Although it would depend on what the task is, what is the most efficient language to use for web development? When working on side projects, I always struggled with finding the best platform(s) to host them. How do we know whether one platform is better than the other?


---


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)
*    If I had a few more hours to work on this project, I would add more additional features to the game and completely change it. Instead of just 4 buttons, I would add more and make it similar to a memorization game. Additionally, I would display the number of guesses the user has for each sequence. I noticed that this game had a set number of sequences, I would change this to infinite. I would also add a scoreboard that stores the top 5 high scores. To make this game more competitive, I would also work on adding a multiplayer mode.


## License

    Copyright Shivasree Margam

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
