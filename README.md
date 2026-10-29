# Bacon Byte L4: Git & the FRC Project

## Tonight's mission
Add your name to the robot's roll call, get it merged, and watch it print in the sim.

## Setup (once)
1. Accept the collaborator invite in your email
2. `git clone https://github.com/thegreatsantini/WPILib-leason.git`
3. Open the folder in **WPILib VS Code**

## Your workflow (every change, every time)
1. `git checkout main` then `git pull` to get the latest
2. `git checkout -b yourname/what-youre-doing`
3. Make your change
4. `git add .`
5. `git commit -m "what you changed"`
6. `git push -u origin yourname/what-youre-doing`
7. On GitHub: **Compare & pull request** → into `main`

**Never push straight to `main`.** 

## Your task
In `Robot.java`, find the roll call comment and add:
    System.out.println("YOUR NAME was here");
Run the sim: `Ctrl+Shift+P` → **WPILib: Simulate Robot Code**

## Where things live
| File | What it does |
|---|---|
| `Robot.java` | The robot's heartbeat. Mostly stays empty. |
| `RobotContainer.java` | Wires buttons to commands. |
| `Constants.java` | Numbers that never change (ports, IDs). |
| `subsystems/` | Classes that own hardware (next week!) |
| `commands/` | Things the robot does |

## When Git yells at you
| Error | Fix |
|---|---|
| `nothing added to commit` | You forgot `git add .` |
| `src refspec main does not match any` | You haven't committed anything yet |
| `rejected... fetch first` | `git pull`, then push again |
| `CONFLICT` | Don't panic. Raise your hand. |

## Words
- **Commit**: a save point
- **Branch**: your own copy to experiment on
- **Push**: send your commits to GitHub
- **Pull request (PR)**: "please merge my branch into main"