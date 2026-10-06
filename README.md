# CS 1430 — Assignment 1: Hello, World!

> **Use this template — do NOT click Fork.**
> Click the green **Use this template** button at the top of this page, then
> **Create a new repository**. Name it `cs1430-a01-YOUR-GITHUB-USERNAME` and
> leave it set to **Public**.

This assignment is not really about Python. It is about proving that Python,
Git, GitHub, and VS Code are installed on your computer and talking to each
other. You will make one small change to a program, save it to GitHub, and
prove it worked.

---

## What you are changing

`main.py` prints a big ASCII-art "Hello, World!" banner.

**Your job is to add your name to what the program prints.**

Two rules:

1. **Do not change anything between the two `DO NOT EDIT` lines.** The banner
   stays exactly as it is.
2. **Add at least one `print()` statement** below the `ADD YOUR CODE BELOW THIS
   LINE` comment at the bottom of the file, and make your name show up when the
   program runs.

Plain text is completely fine:

```python
print("Made by Dan Example")
```

ASCII art is better, and you do not have to make it by hand. Ask Copilot:

> *Make my name "Dan Example" as ASCII art I can print from Python. Use only
> plain letters and simple characters, no backslashes.*

Then print it the same way the banner is printed. **Three quotation marks start
the string, your art goes in the middle, three more end it:**

```python
MY_NAME = """
DDDD    A   N   N
D   D  A A  NN  N 
D   D AAAAA N N N 
D   D A   A N  NN
DDDD  A   A N   N 
"""

print(MY_NAME)
```

That is exactly the pattern `BANNER` uses in `main.py`. Copy the shape, swap in
your own art.

**If your art has backslashes in it.** Some ASCII-art letters are drawn with the
`\` character, and Python treats a backslash as an instruction rather than as
art. Two fixes, either is fine:

- Ask Copilot for art without backslashes, as in the prompt above, or
- Put the letter `r` right before your opening quotes:

```python
MY_NAME = r"""
   art with \ characters in it
"""
```

The banner in `main.py` uses letters that need no backslashes, which is why it
does not need the `r`. `check.py` will tell you if you hit this.

---

## Steps

1. Click **Use this template → Create a new repository**. Name it
   `cs1430-a01-YOUR-GITHUB-USERNAME`. Keep it **Public**.
2. Clone your new repository to `C:\CS1430\`.
   **Not** Documents, **not** Desktop, **not** anywhere OneDrive syncs.
3. In VS Code, open the **folder** you just cloned. Not a single file — the
   whole folder.
4. Open `main.py`. Add your `print()` below the `ADD YOUR CODE` line. Save.
5. Run `check.py`.
   **It is supposed to fail the last line the first time.** Read what it says.
6. Stage your change, write a commit message, and **push**.
7. Run `check.py` again. When every line says `PASS`, it writes a file called
   `SUBMISSION.txt` into your folder.
8. Upload `SUBMISSION.txt` in Canvas and answer the reflection questions.

---

## Running the checker

Open `check.py` in VS Code and press the **Run** button (the ▷ in the top
right), or type this in the VS Code terminal:

```
python check.py
```

You do not need to install anything. There is no `pip install` in this
assignment.

If a line says `FAIL`, **fix the first one and run it again.** Do not try to fix
all of them at once. Each failure prints a hint on the line below it.

---

## What you turn in

| | |
|---|---|
| **In Canvas** | `SUBMISSION.txt` (the checker writes it for you) |
| **In Canvas** | Your answers to the four reflection questions |
| **On GitHub** | Your pushed commit — the checker confirms this for you |

`SUBMISSION.txt` is created automatically. You never need to take a screenshot
of your terminal, and you should not edit the file by hand — it records your
repository address and your commit, and those are checked against GitHub.

---

## If you get stuck

- **`'git' is not recognized`** — close every terminal, then close and reopen
  VS Code. The install finished after your terminal opened.
- **`main.py is in this folder` fails** — you opened the file instead of the
  folder. In VS Code: **File → Open Folder**, and pick the folder you cloned.
- **A backslash warning, or `main.py` stops running after you add your art** —
  your ASCII art contains `\` characters. Put the letter `r` just before your
  opening triple quotes: `MY_NAME = r"""`.
- **`The ASCII art is unchanged` fails** — something between the `DO NOT EDIT`
  lines got changed. Open this template repository on GitHub, copy that section,
  and paste it back over yours.
- **`Your commit is pushed to GitHub` fails** — you committed but did not push.
  Committing saves your work on this computer. Pushing sends it to GitHub.
- **Anything else** — the Assignment 1 Troubleshooting page in Canvas is
  organized by the exact message you are seeing.

If you do not have a computer you can install software on, contact your
instructor. Do not wait.
