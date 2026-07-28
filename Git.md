
<details>
<summary><strong>1. What is Git, and why is it used?</strong></summary>

```text
Git is a distributed version control system that helps us track changes in source code and collaborate with multiple developers.

Why we use it:

• It maintains version history.
• Multiple developers can work on different features simultaneously using branches.
• We can roll back to previous versions if something goes wrong.
• It integrates well with CI/CD tools like Jenkins and GitHub Actions.
```

</details>

<details open>
<summary><strong>2. What is the difference between a Centralized Version Control System (CVCS) and a Distributed Version Control System (DVCS)?</strong></summary>

```text
The main difference is where the version history is stored.

Centralized Version Control System (CVCS):
• There is one central server that stores the entire repository.
• Developers connect to that server to pull and push changes.
• If the server goes down, collaboration is affected.

Distributed Version Control System (DVCS):
• Every developer has a complete copy of the repository, including the full history.
• Developers can work offline.
• It provides better reliability and faster operations.
```

</details>


<details>
<summary><strong>Explain the Git architecture.</strong></summary>

```text

## Interview Answer

> **Git follows a distributed architecture, which means every developer has a complete copy of the repository, including the entire commit history. This makes Git fast, reliable, and allows developers to work offline.**

### Git Architecture

```
                  Remote Repository
             (GitHub / GitLab / Bitbucket)
                       ▲
                 git push / git pull
                       │
                Local Repository (.git)
               (Complete commit history)
                       ▲
                  git commit
                       │
                Staging Area (Index)
                       ▲
                   git add
                       │
                Working Directory
          (Where we create/edit files)
```

### Explain Each Component

#### 1. Working Directory

* This is where we write or modify our code.
* Any changes we make are initially only in the working directory.

**Example:**

> I edit `app.py` to add a new feature.

---

#### 2. Staging Area (Index)

* The staging area acts as a **temporary holding area**.
* We use `git add` to move selected changes here before committing.

**Command:**

```bash
git add app.py
```

**Why it's useful:**

> It lets us choose exactly which changes should be included in the next commit.

---

#### 3. Local Repository

* When we run `git commit`, Git saves the staged changes permanently in the local repository.
* The local repository stores the **entire project history**.

**Command:**

```bash
git commit -m "Added login feature"
```

---

#### 4. Remote Repository

* This is the shared repository hosted on platforms like GitHub or GitLab.
* It is used for collaboration with other developers.

**Commands:**

```bash
git push origin main
```

```bash
git pull origin main
```

---

## Workflow

```
Modify Code
     │
     ▼
Working Directory
     │
 git add
     ▼
Staging Area
     │
git commit
     ▼
Local Repository
     │
git push
     ▼
Remote Repository
```

---

## One-Line Answer (if the interviewer asks briefly)

> **Git architecture consists of four main components: the Working Directory, Staging Area, Local Repository, and Remote Repository. Changes move from the Working Directory → Staging Area → Local Repository → Remote Repository, enabling efficient version control and collaboration.**

---

</details>

<details>
<summary><strong>Question</strong></summary>

```text
Answer

Key Points:

• Point 1
• Point 2
• Point 3
• Point 4
```

</details>

