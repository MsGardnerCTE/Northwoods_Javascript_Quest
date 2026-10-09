# Nighthawk JavaScript Quest

A three-level Sphero JavaScript activity for Ms. Gardner's Fundamentals of Computing class. Uses the exact blue theme, Northwoods logo, and CTE logo from the earlier Nighthawk HTML Quest.

## Put the website on GitHub Pages

1. Create a new GitHub repository named `nighthawk-javascript-quest`.
2. Extract this ZIP. Open the folder inside it.
3. Choose **Add file > Upload files** in the repository. Upload the files inside the extracted folder, including both JPG logos. `index.html` should be at the repository's top level.
4. Commit the files.
5. Open **Settings > Pages**. Choose **Deploy from a branch**, select **main** and **/ (root)**, and save.
6. When GitHub displays the published link, open it and share that link with students.

The site uses HTML, CSS, and JavaScript with local images. There are no external fonts, packages, logins, or paid services. It can also be opened locally using `index.html`. For a single-file local preview, open `Preview.html`.

## The student experience

- Level 1: Hello World. Six code-click questions start with the message argument, then the scrolling function name. Additional questions identify color, number, boolean, and the startProgram function.
- Level 2: Conditionals. Students click the condition, the true action, and the else action. Three balloon predictions use speeds 0, 72, and exactly 1. Students then edit the conditional and demonstrate a false test for a stopped robot, changes to all three roll arguments, and a new LED color.
- Level 3: Loops. Students modify the repeat count to five, change blocking to false, increase the delay to four seconds, choose BonusSuper, and insert the yellow main LED command between sound and delay.
- Twenty challenges award 100 points each. Incorrect answers give hints and allow retries. Navigation unlocks each level after the previous one is completed. Students can revisit unlocked levels without earning duplicate points.
- There is no timer. Progress lasts for the current page session. Refreshing starts a new session. Students can download their final results and exit ticket.

## Robot use and teaching notes

The website previews behavior on screen. It does not connect to or control a physical robot. Students use **Copy code** or **Download code**, then paste the program into the JavaScript canvas in Sphero Edu and run it with a connected robot.

The editor checks the demonstrated program structures. It supports the edits requested in this lesson, rather than arbitrary JavaScript. Extra exploration beyond those structures belongs in Sphero Edu. Preview limits are listed in validation feedback.

The supplied conditional had `async async`; the duplicate keyword has been removed. `setMainLed` changes the main LED, so that challenge says main LED rather than matrix. To teach matrix color, substitute the appropriate matrix command for your robot in a future activity.

`Sound.Animal.play(true)` selects a random animal sound. The true argument waits for playback to finish. False starts playback and continues immediately; it does not mute audio. Sphero Edu plays these sounds on the programming device. The browser model illustrates command order with text and compressed timing, without using actual Sphero sound recordings. Physical sound lengths and motion can vary.

The condition `getSpeed() < 1` is checked once. For the normal stopped scenario, 0 makes it true. One valid edit that triggers only else for that scenario is `getSpeed() > 1`. Students can restore the original comparison to demonstrate the modified roll at speed 0, then choose a current speed of 72 to demonstrate the new else color. A negative speed also satisfies the original less-than comparison, so this is not a general test of whether the robot is stopped in all circumstances.

## References

- [Sphero JavaScript sounds](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/sounds)
- [Sphero JavaScript movement](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/movement)
- [Sphero JavaScript lights](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/lights)

## Included files

`index.html`, `style.css`, `quest.css`, `game.js`, `northwoods.jpg`, `cte.jpg`, `Preview.html`, and this guide.
