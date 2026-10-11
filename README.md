# Nighthawk JavaScript Mastery Games

Three independent daily games for Ms. Gardner's Fundamentals of Computing class. The original Northwoods blue theme and Northwoods/CTE logos remain. Students can go directly to any game. Each game has five mastery rounds and its own daily Challenge Complete screen.

## Update the website you already created

1. Download and extract the ZIP.
2. Open your existing `nighthawk-javascript-quest` repository on GitHub.
3. Select **Code > Add file > Upload files**.
4. Open the extracted folder. Upload these files from inside it:
   - `index.html`
   - `style.css`
   - `quest.css`
   - `game.js`
   - `arcade.js`
   - `northwoods.jpg`
   - `cte.jpg`
5. Click **Commit changes**. `index.html` must appear at the repository's top level. Upload the individual files rather than the ZIP or the enclosing folder.
6. An already-enabled GitHub Pages website publishes this committed update. Refresh the website after publication completes. If you still see the old version, use Ctrl+Shift+R.

Open `Preview.html` to try the whole game as a single local file. That preview file is optional for GitHub hosting.

For a new repository, choose **Settings > Pages > Deploy from a branch**, select **main** and **/ (root)**, then save.

## Daily games and links

| Day | Game | Completion requirement |
|---|---|---|
| 1 | Hello World | Master five balloon rounds |
| 2 | Conditionals | Master five prediction rounds and complete three guided question steps |
| 3 | Loop Launch | Complete five editing tasks and master five loop rounds |

Each day's completion is independent. Students do not have to complete another day's game to earn the current day's completion screen.

Add `#game1`, `#game2`, or `#game3` to the website address to open the preferred game directly. For example, `https://msgardnercte.github.io/nighthawk-javascript-quest/#game2`.

All games are unlocked from the home screen. Within each game, students must master the current round to access the next round.

## Mastery points and penalties

| Game | Correct | Incorrect | Required to advance |
|---|---:|---:|---|
| Hello World | +10 | -10 | At least 100 round points and 10 correct pops |
| Conditionals | +20 | -10 | At least 100 round points and 5 correct answers |
| Loop Launch | +20 | -10 | At least 100 round points and 5 correct answers |

An incorrect answer always deducts points. Round points can go below zero, so every mistake must be recovered through additional correct answers. For example, five correct conditional answers and one incorrect answer give 90 points; a sixth correct answer gives 110 points and meets the goal. Round points reset when the round is mastered. Overall accuracy continues accumulating throughout the game.

Hello World also deducts 10 points when a matching target balloon escapes. Letting a decoy escape has no penalty. Clicking the same balloon twice does not award twice. Matching values are judged against the currently displayed function call and prompt.

Conditionals and Loop Launch allow exactly one attempt per question. An incorrect click immediately clears all three answer balloons, deducts 10 points, breaks the streak, and shows the correct answer with an explanation. Clicking the other balloons cannot recover points for that question. Students choose **Next scenario** to continue, or **Round mastered** once they meet both mastery requirements.

There is no countdown or automatic advancement based on time. Questions in Conditionals and Loops remain available until answered. Hello World is still a fast movement game with missed-target penalties, but its progression depends on mastery points. Completion time varies with accuracy, reading, and editing pace.

## Final score for student rewards

Each completed daily game earns a final score out of 1,000:

- 500 completion points for mastering all five rounds.
- Up to 500 accuracy points, rounded from `500 × correct / (correct + wrong clicks + missed targets)`.

A perfect completed game earns 1,000. A completed game with 90% accuracy earns 950. Bonus streak points do not bypass the mastery requirements. Streaks are displayed for motivation, but do not add to the reward score.

Unscored introductory practice and editing tasks support learning without changing the final accuracy score. Reward scores use scored balloon rounds only. Each game has its own final score, so compare students within the same daily game.

## Completion screen and teacher review

Students enter a name when starting a game. Each completion screen shows:

- **Hello World Challenge Complete!**, **Conditionals Challenge Complete!**, or **Loop Launch Challenge Complete!**
- Student name and completion date/time.
- Final score out of 1,000.
- Accuracy and **5 / 5 rounds mastered**.
- Correct answers, wrong clicks, missed targets, and best streak.
- A table of each round's mastery points, correct answers, and mistakes.
- An exit ticket and downloadable text results.

Students can show you the completion screen, submit a screenshot to Canvas, or download and submit the text results. There is no shared online teacher leaderboard. Reports and progress are kept in the current browser, so students should submit their own reports for classwide comparison.

## Game 1: Hello World

Six unscored code-click practice questions introduce functions and arguments. Then:

1. Hello World arguments only.
2. Hello World function names only.
3. Mixed arguments from familiar Sphero function calls.
4. Mixed function names from those calls.
5. Mixed mastery, alternating function-name and argument targets between waves.

Mixed calls include `scrollMatrixText`, `roll`, `delay`, `setMainLed`, `spin`, `speak`, and `setDisplayImage`. The full mixed reference contains all of these calls. It stays fixed during the round, so balloons always match the visible reference. The entire RGB object counts as one argument. `startProgram` is a function name in the wrapper. Keywords are distractors.

Balloons keep dropping at about 0.9-second intervals wherever there is room. The game does not wait for a batch to clear. Falling speed starts at 90 pixels/second and increases by 12 each round. Round 5 puts a FUNCTION or ARGUMENT target badge on each balloon: pop only code pieces that match their own badge. That allows continuous drops without changing the target for balloons already on screen.

## Game 2: Conditionals

Three unscored code-click questions introduce the original if/else example. Every scored round shows a different reference:

| Round | Condition | Roll action | ELSE LED |
|---|---|---|---|
| 1 | `getSpeed() < 20` | heading 0, speed 60, duration 2 | Blue |
| 2 | `getSpeed() > 50` | heading 90, speed 100, duration 3 | Red |
| 3 | `getSpeed() <= 40` | heading 180, speed 80, duration 4 | Green |
| 4 | `getSpeed() >= 72` | heading 270, speed 120, duration 2 | Yellow |
| 5 | `getSpeed() === 100` | heading 45, speed 90, duration 5 | Purple |

Scenarios use varied speeds such as 12, 20, 35, 40, 50, 51, 72, 99, 100, and 120. Each round includes boundary values that test equality. Only one branch runs. The action balloons include the roll arguments and LED color shown in that round's actual reference.

After the scored rounds, students complete guided questions instead of editing conditional code:

1. Choose the condition that sends a stopped robot to ELSE.
2. Identify direction, speed, and duration with three short questions.
3. Predict the main LED color when ELSE runs.

Each question displays the exact program and scenario. Choosing an answer reveals the correct explanation and a matching robot preview. The green LED question explicitly uses speed 72, making `getSpeed() < 1` false so ELSE runs. Wrong answers end that attempt and offer a fresh guided try. Guided practice is unscored; the reward score remains based on the scored five rounds. After all guided questions are correct, students can open the daily Challenge Complete screen.

## Game 3: Loop Launch

The loop editing lab preserves all five requested changes: five repetitions, false blocking, four-second delay, BonusSuper sound, and the added yellow LED command.

An inline continuation panel sits beside the checklist. When all five tasks have been checked and the current program has valid syntax, it displays **All five steps complete!** and enables **Continue to Balloon Challenge →**. The same action is also available below the lab.

Each scored round then has a slightly different reference:

1. Three repetitions, animal sound, true blocking, two-second delay.
2. Five repetitions, BonusSuper sound, true blocking, one-second delay.
3. Four repetitions, animal sound, false blocking, four-second delay.
4. Three repetitions with a blue LED command added inside the loop.
5. Five repetitions with BonusSuper sound, false blocking, a yellow LED command, and four-second delay.

Question types vary within each round: repetitions, starting/last/stopping counter values, command order, selected sounds, blocking, per-repetition/total delay, repeated LED behavior, and full-program predictions. The editing draft can be copied to Sphero Edu separately; the scored rounds use the five stated reference programs so each round looks different.

## Progress, accessibility, and robot testing

Games save separate student names, progress, points, accuracy, editing drafts, completed tasks, and results in this browser. Switching games or reloading resumes the current stage. Replay resets only that game. This update starts fresh mastery progress using a new storage key; previous timed-game progress is not counted as mastery.

Pause stops balloon movement. Hiding the browser tab automatically pauses an active balloon round. Balloons are buttons supporting mouse, touch, and keyboard Space/Enter. A system reduced-motion preference uses stationary targets in Hello World, with target expiry still applying. Prediction balloons remain available until answered.

The website models behavior on screen. Copy or download edited code and run it in Sphero Edu with a connected robot. The editing checks support the demonstrated program structures rather than arbitrary JavaScript. Free exploration beyond those structures belongs in Sphero Edu.

`Sound.Animal.play(true)` selects a random animal sound. True waits for playback; false starts sound and continues without waiting. False does not mute audio. These functions play sound through the programming device. The lab preview uses compressed illustrative timing and no Sphero audio recordings.

## Validation

JavaScript syntax and a DOM event harness check mastery gates, incorrect-answer recovery, no timer-based advancement, one-attempt protection, mixed function/argument targets, five unique conditional references, five unique loop references, boundary scenarios, all editing tasks, independent daily completion screens, accuracy scoring, pause, student-name entry, saved partial progress, restored reports, and replay isolation. Full browser rendering could not be tested in the build environment.

## References

- [Sphero sounds](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/sounds)
- [Sphero movement](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/movement)
- [Sphero lights](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/lights)
- [GitHub Pages publishing](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Latest update

- Continuous Hello World drops in every round, with no batch-clear pauses.
- Added spin, speak, and setDisplayImage examples to rounds 3–5.
- Replaced conditional code editing with guided Q&A and branch/color previews.
- Added a visible, enabled Loop Launch continuation button next to completed tasks.
- Existing completed Conditionals sessions reopen at the new guided questions; other saved game progress remains. Use **Replay this game** on a completion screen to start a fresh test.
- Additional checks cover continuous spawning in all rounds at desktop/mobile sizes, both motion preferences, the green ELSE preview, and the inline loop continuation action.

Display reference: [Sphero display commands](https://sites.google.com/sphero.com/sphero-edu-javascript-wiki/display). The `setDisplayImage` example targets BOLT+.
