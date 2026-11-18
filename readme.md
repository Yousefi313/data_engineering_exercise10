# Data Engineering Exercise 10 – Git with Remote and Team Workflow

This repository contains the completed work for Exercise 10 of **Programming 1** under **Prof. Dr. Amy Siu** at **Berliner Hochschule für Technik (BHT)**. 

The main objective of this exercise is to practice using a remote Git repository in a team setting, manage remote synchronization, and handle merge conflicts.

---

## 👥 Solo Team Workflow ("Team of 1")
As permitted for students unable to form a traditional multi-person group, this exercise was executed using a **"team of 1" simulation strategy**[cite: 1]. 
* Two independent local clones (`repo-me` and `repo-teammate`) were created from this single remote repository to simulate two distinct team members collaborating simultaneously[cite: 1].

---

## 🛠️ Scenarios Practiced & Implemented

### Scenario 1: Non-Overlapping Changes (Different Files)
* **Action**: Added code independently across different files (`fileA.py` in `repo-me` and `fileB.py` in `repo-teammate`)[cite: 1].
* **Result**: Successfully pushed independent features and synchronized the remote repository without needing actual code merges.

### Scenario 2: Overlapping Files with Easy Auto-Merge
* **Action**: Added `function_x` at the top of `fileA.py` in `repo-me` and `function_y` at the bottom of `fileA.py` in `repo-teammate`[cite: 1].
* **Result**: Demonstrated Git's capability to intelligently and automatically merge changes located in different sections of the same file.

### Scenario 3: Conflicting Changes (Same Line Conflict)
* **Action**: Both local clones modified the exact same line of code in `fileA.py` concurrently[cite: 1]. 
* **Result**: Triggered a merge conflict divergence, allowing for manual inspection and resolution using Git conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`).

---

## 📂 Repository Structure
```text
├── fileA.py           # Used for testing file changes, function additions, and merge conflicts
├── fileB.py           # Used for testing independent file addition (Scenario 1)
└── README.md          # Project documentation