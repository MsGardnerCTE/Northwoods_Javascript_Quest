# Nighthawk JavaScript Arcade

Three independent classroom games using the original Northwoods blue theme and Northwoods/CTE logos. Students may choose game 1, 2, or 3 immediately. There are no locked games or prerequisites.

## Update your existing GitHub website

1. Extract the ZIP.
2. Open your existing `nighthawk-javascript-quest` repository on GitHub.
3. Select **Code > Add file > Upload files**.
4. Open the extracted folder and drag the website files into GitHub: `index.html`, `style.css`, `quest.css`, `game.js`, the new `arcade.js`, `northwoods.jpg`, and `cte.jpg`.
5. Commit the changes. Keep `index.html` at the repository's top level. Upload files from inside the folder rather than the ZIP or the entire enclosing folder.
6. If GitHub Pages is already enabled, it publishes the committed update automatically. Refresh the student website once publication completes. Use Ctrl+Shift+R if your browser displays the old version.

For a new repository, enable **Settings > Pages > Deploy from a branch**, choose **main**, choose **/ (root)**, and save.

For a local single-file preview, open `Preview.html`. The separate files above are the files to upload to GitHub.

## Choose any game

The home screen has three play buttons. Navigation buttons also let students switch games anytime. Each game saves its own score, editing draft, completed tasks, active time, and completed rounds in this browser's local storage. Returning to a game restores the stage and remaining round time. This is a local record on that browser, not a teacher dashboard or cross-device login. Shared devices share that record. Replay resets only the selected game.

Append `#game1`, `#game2`, or `#game3` to your website's URL to open that game directly. For example: `https://msgardnercte.github.io/nighthawk-javascript-quest/#game2`.

## Time and activities

| Game | Activities | Typical classroom time |
|---|---|---|
| 1: Hello World Pop | Six code-click practice questions; seven 60-second balloon rounds; exit ticket | About 8–10 minutes |
| 2: If/Else Balloon Dash | Six code/balloon practice questions; five 60-second prediction rounds; three editing tasks; exit ticket | About 8–10 minutes |
| 3: Loop Launch | Five editing tasks; five 60-second balloon rounds based on the edited loop; exit ticket | About 7–10 minutes |

These are pacing estimates. Reading, editing, and reflection take different amounts of time for different students. The actual timed balloon play is seven minutes for Hello World and five minutes for each other game. No rounds end early because a point target is reached. Students manually start each round, with a short review between rounds. Pauses, round setup, round reviews, and time on a hidden browser tab do not advance the active-play timer.

## Game 1: Hello World Pop

Students first click the message argument, the scrolling function name, the color object, the number argument, the boolean, and the defined startProgram function. Then they play seven different one-minute rounds:

1. Message argument
2. Scrolling function name
3. Full RGB color argument
4. Number argument 15
5. Boolean argument true
6. Start function name
7. Mixed challenge: all arguments, avoiding functions and keywords

Balloons fall continuously with relevant code pieces and decoys. Drops speed up gradually across rounds. There is no need to click decoys.

## Game 2: If/Else Balloon Dash

The code practice introduces the condition and alternate actions. Timed rounds show a current-speed scenario and a program reference, with falling action balloons. Early rounds use the original code and speeds such as 0, 1, and 72. Later rounds vary roll arguments and comparisons. The displayed program always reflects those changes. Students must inspect the actual code rather than memorize that speed 0 always means roll.

The editing lab retains all three challenges: trigger only ELSE for the stopped scenario, change all three roll arguments and preview IF, and change the ELSE main LED color and preview ELSE. The supplied duplicate `async` has been corrected. `setMainLed` changes the main LED, so the lab uses that label rather than matrix.

## Game 3: Loop Launch

All five requested edits remain: five repetitions, false blocking, four-second delay, BonusSuper sound, and the added yellow LED command. Students then enter five timed balloon rounds based on their actual edited program:

1. Repetitions and counter values
2. Sound waiting and continuation
3. Per-repetition and total delay time
4. LED and sound behavior
5. Mixed loop questions

Questions vary within rounds. The screen model in the lab demonstrates the command order, light changes, and repetition count. The balloon questions read the selected repeat count, wait argument, delay, sound, and LED command from the edited program.

## Scoring and controls

- Correct balloon: +25 points.
- Every five correct pops in a row: +50 streak bonus.
- Wrong balloon: -10 points, score never below zero.
- Missed target: -5 points.
- Code/tutorial/lab milestone: +100 points, once per milestone per game.
- Every completed game shows points, correct pops, best streak, active time, and a downloadable exit ticket.
- Pause freezes both the timer and balloons. Hiding the browser tab automatically pauses an active round.
- Balloons are native buttons, supporting touch, mouse, and keyboard Space/Enter.
- A system reduced-motion preference uses stationary targets with timed expiry.

## Robot testing

This website previews behavior and checks the demonstrated program structures. It does not connect directly to a robot or execute arbitrary JavaScript. Students copy or download code from the editing lab and run it in Sphero Edu with a connected robot. Free exploration outside the supported template belongs in Sphero Edu.

`Sound.Animal.play(true)` chooses a random animal sound. True waits for sound completion; false continues immediately while audio plays. False does not mute sound. These Sphero Edu functions play audio through the programming device. The screen model uses compressed illustrative timing and no Sphero audio recordings. Motion on a robot depends on aiming and the surface.

## References

- [Sphero sounds](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/sounds)
- [Sphero movement](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/movement)
- [Sphero lights](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/lights)
- [GitHub Pages publishing](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Validation

JavaScript syntax and a DOM event harness check all tutorial/editing paths, independent access, seven/five/five full timed rounds, pause/resume, score isolation, draft validation, saved progress, reload, replay isolation, mid-round restoration, duplicate-pop protection, and code validation. A full browser rendering test was unavailable in the build environment.
