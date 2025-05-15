## Beginner Python Course – *Foundations in Five Lessons*

### 0  Course snapshot

* **Audience**  Absolute beginners—no prior coding experience.
* **Duration**  5 × 90-minute sessions (live or self-paced).
* **Structure**  Concept burst → live demo → guided exercise → recap quiz.
* **Tools**  Python 3.12+, any editor/IDE (VS Code recommended), terminal/command prompt. Alternatively online python [https://www.online-python.com/](https://www.online-python.com/)

---

### Lesson 1  Hello World

**Objectives**

1. Install Python and verify the version.
2. Write and run your first script from the terminal and the editor.
3. Understand the edit-save-run-debug cycle.

**Demo**

```bash
python --version          # macOS/Windows/Linux
python hello.py
```

```python
# hello.py
print("Hello, World!")
```

**Hands-on (10 min)**

* Replace the greeting with your own name.
* Run the file both from the command line and via the IDE “Run” button.

---

### Lesson 2  Primitive Data Types — `str`, `int`, `float`

**Objectives**

1. Recognise core types and why they matter.
2. Perform arithmetic with `int` / `float`.
3. Slice and format strings.
4. Inspect types with `type()`.

**Key snippets**

```python
name = "Ada Lovelace"      # str
age  = 30                  # int
price = 19.95              # float
bmi  = 68 / (1.7 ** 2)     # float math
print(f"{name} is {age} and the BMI is {bmi:.1f}")
```

**Practice (20 min)**

* Build a simple temperature converter (°C ↔ °F).
* Call `type()` on every variable and inspect the output.

---

### Lesson 3  Loops — `for` and `while`

**Objectives**

1. Iterate over sequences with `for … in`.
2. Generate sequences with `range()`.
3. Control repetition with `while` and loop-exit conditions.
4. Use `break` and `continue` responsibly.

**Illustrations**

```python
# For loop – shopping list
for item in ["eggs", "milk", "bread"]:
    print("Buy", item)

# While loop – countdown
seconds = 5
while seconds:
    print(seconds)
    seconds -= 1
print("Liftoff!")
```

**Exercise (25 min)**

* Print every multiple of 3 from 0 to 30 using both `for` and `while`.
* *Stretch*: create an infinite `while` loop that stops on user input `"quit"`.

---

### Lesson 4  Conditionals — `if`, `elif`, `else`

**Objectives**

1. Compare values (`==`, `!=`, `<`, `>`, etc.).
2. Chain logic with `elif`.
3. Combine conditionals inside loops for simple state machines.

**Demo**

```python
speed = int(input("Speed in km/h: "))

if speed > 110:
    print("Slow down! Too fast.")
elif speed >= 80:
    print("Within highway limit.")
else:
    print("Under limit—safe driving.")
```

**Exercise (30 min)**

* Write a “traffic light” program: input `red`, `amber`, or `green`; output `"Stop"`, `"Prepare"`, or `"Go"`.
* Combine with a `while` loop so the prompt repeats until the user types `"exit"`.

---

### Lesson 5  Collections — `list` & `dict`

**Objectives**

1. Create, index, and slice lists.
2. Mutate lists with `append`, `pop`, and list comprehension.
3. Store key–value pairs in dictionaries; access and update entries.
4. Iterate over collections with `for` loops.

**Core examples**

```python
# List
scores = [78, 92, 61, 88]
average = sum(scores) / len(scores)

# Dict
student = {"name": "Ada", "age": 30, "scores": scores}
for key, value in student.items():
    print(key, "=>", value)
```

**Practice (30 min)**

* Build a contact book: continuously ask for a name and phone number, store them in a dictionary, list all contacts when the user types `"list"`, and quit on `"q"`.
* *Stretch*: allow updating an existing contact’s phone.

---

### Capstone Mini-Project – **Number Guessing Game**

Integrates input/output, data types, loops, conditionals, and collections.

**Specs**

* Randomly choose an integer 1-100.
* Player guesses; program replies *Too high / Too low / Correct*.
* Track the number of attempts in a list; show the history on success.
* Limit to 7 tries; reveal the number if the player loses.

---

### Wrap-up & Next Steps

* 10-question quiz covering all five lessons.
* Encourage creating a GitHub repo to store exercises.
* Recommend advancing to functions, error handling, and modules.