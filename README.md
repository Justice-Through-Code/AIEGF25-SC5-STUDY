# AIEGF25-SC5-STUDY

# Skills Check 5 - Study Guide
## Your Path to Graduation 🎓

---

## 📋 What Is Skills Check 5?

Skills Check 5 is your **graduation assessment**. It validates everything you've learned across the program and determines your readiness to advance to AI Foundations.

**Format:** 20-minute 1:1 proctored session
- Part 1: Explain your thinking (verbal)
- Part 2: Demonstrate your skills (coding or debugging)
- Part 3: Read and understand code (trace)

**What you need:** 75/100 to advance

---

## 🗺️ Your Study Path

This guide follows the same journey you took through the program. Start at the beginning and work your way through—each section builds on the last.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│                        YOUR LEARNING JOURNEY                            │
│                                                                         │
│  ┌──────────────┐    ┌──────────────┐    ┌──────────────┐              │
│  │   PHASE 1    │    │   PHASE 2    │    │   PHASE 3    │              │
│  │              │    │              │    │              │              │
│  │  Thinking &  │───▶│    Python    │───▶│   Applied    │              │
│  │   Planning   │    │  Foundations │    │    Python    │              │
│  │              │    │              │    │              │              │
│  └──────────────┘    └──────────────┘    └──────────────┘              │
│         │                   │                   │                      │
│         ▼                   ▼                   ▼                      │
│  ┌──────────────┐    ┌──────────────┐    ┌──────────────┐              │
│  │ • Flowcharts │    │ • Variables  │    │ • Safe data  │              │
│  │ • Breaking   │    │ • Data types │    │   access     │              │
│  │   down       │    │ • Functions  │    │ • Error      │              │
│  │   problems   │    │ • Loops      │    │   handling   │              │
│  │ • AND/OR     │    │ • Lists &    │    │ • JSON       │              │
│  │   logic      │    │   Dicts      │    │ • APIs       │              │
│  └──────────────┘    └──────────────┘    └──────────────┘              │
│                                                                         │
│                              │                                          │
│                              ▼                                          │
│                    ┌──────────────────┐                                │
│                    │   SKILLS CHECK   │                                │
│                    │        5         │                                │
│                    │                  │                                │
│                    │  ALL SKILLS      │                                │
│                    │  COMBINED        │                                │
│                    └──────────────────┘                                │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

# 📘 PHASE 1: Thinking & Planning

## Why This Matters

Before you write a single line of code, you need to **think through the problem**. SC5 tests whether you can break down a problem and anticipate issues before coding.

---

## 1.1 Breaking Down Problems

**The skill:** Taking a complex task and splitting it into smaller steps.

**Example scenario:**
> "Build something that checks if a user can access premium content"

**How to break it down:**

```
┌─────────────────────────────────────────────────────┐
│                 COMPLEX PROBLEM                     │
│         "Can user access premium content?"          │
└─────────────────────────────────────────────────────┘
                         │
                         ▼
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
   ┌─────────┐     ┌─────────┐     ┌─────────┐
   │ Step 1  │     │ Step 2  │     │ Step 3  │
   │         │     │         │     │         │
   │ Get the │     │ Check   │     │ Return  │
   │ user    │     │ their   │     │ yes/no  │
   │ data    │     │ status  │     │ answer  │
   └─────────┘     └─────────┘     └─────────┘
        │                │                │
        ▼                ▼                ▼
   What could       What could       What format
   go wrong?        go wrong?        should this be?
```

**Practice thinking:**

When given a problem, ask yourself:
1. What are the **inputs**? (What data do I start with?)
2. What are the **steps**? (What do I need to do?)
3. What is the **output**? (What should I return?)
4. What could **go wrong**? (What errors might happen?)

---

## 1.2 Boolean Logic: AND vs OR

**The skill:** Understanding when both conditions must be true vs. when just one is enough.

### AND Logic

**Both conditions must be true.**

```
┌─────────────────────────────────────────────────────┐
│                      AND                            │
│                                                     │
│     Condition A          Condition B                │
│         │                    │                      │
│         ▼                    ▼                      │
│     ┌───────┐            ┌───────┐                 │
│     │ True? │            │ True? │                 │
│     └───┬───┘            └───┬───┘                 │
│         │                    │                      │
│         └────────┬───────────┘                      │
│                  ▼                                  │
│         ┌───────────────┐                          │
│         │ BOTH must be  │                          │
│         │ True for      │                          │
│         │ result = True │                          │
│         └───────────────┘                          │
└─────────────────────────────────────────────────────┘
```

**Real examples:**
- "You can enter **if** you have a ticket **AND** you're on the list"
- "The alarm goes off **if** the door is open **AND** the system is armed"
- "Buy the item **if** it's in stock **AND** it's under budget"

### OR Logic

**At least one condition must be true.**

```
┌─────────────────────────────────────────────────────┐
│                       OR                            │
│                                                     │
│     Condition A          Condition B                │
│         │                    │                      │
│         ▼                    ▼                      │
│     ┌───────┐            ┌───────┐                 │
│     │ True? │            │ True? │                 │
│     └───┬───┘            └───┬───┘                 │
│         │                    │                      │
│         └────────┬───────────┘                      │
│                  ▼                                  │
│         ┌───────────────┐                          │
│         │ EITHER can be │                          │
│         │ True for      │                          │
│         │ result = True │                          │
│         └───────────────┘                          │
└─────────────────────────────────────────────────────┘
```

**Real examples:**
- "Show a warning **if** battery is low **OR** storage is full"
- "Give a discount **if** they're a member **OR** it's a holiday"
- "Send alert **if** temperature is too high **OR** too low"

### Quick Quiz: AND or OR?

1. "A student passes if they score 70+ on the exam AND complete all homework"
   - Answer: **AND** (both required)

2. "Show the error message if username is empty OR password is empty"
   - Answer: **OR** (either triggers it)

3. "Approve the loan if credit score is above 700 AND income is above $50k"
   - Answer: **AND** (both required)

---

## 1.3 Anticipating Errors

**The skill:** Thinking about what could go wrong before it happens.

**Common things that go wrong:**

```
┌─────────────────────────────────────────────────────┐
│              WHAT COULD GO WRONG?                   │
├─────────────────────────────────────────────────────┤
│                                                     │
│  📂 DATA MIGHT BE MISSING                          │
│     • A dictionary key doesn't exist               │
│     • A value is None when you expected a number   │
│     • A list is empty                              │
│                                                     │
│  🔢 DATA MIGHT BE WRONG TYPE                       │
│     • Got a string when you expected a number      │
│     • Got None when you expected a dictionary      │
│                                                     │
│  📁 FILE OPERATIONS                                │
│     • File doesn't exist                           │
│     • Can't write to location                      │
│                                                     │
│  🌐 EXTERNAL DATA                                  │
│     • API returns unexpected format                │
│     • Missing fields in JSON                       │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**Practice:** For any problem, always ask:
- "What if a key is missing?"
- "What if the data is empty?"
- "What should happen when something goes wrong?"

---

## Phase 1 Practice Problems

**Problem 1:** Break this down into steps:
> "Check if a product should be featured on the homepage"

Think about: What data do you need? What conditions matter? What do you return?

<details>
<summary>Sample thinking</summary>

**Steps:**
1. Get the product data
2. Check if it meets the criteria (rating? sales? in stock?)
3. Return True or False

**What could go wrong:**
- Product data might be missing some fields
- Rating might not exist
- Need to handle missing data gracefully
</details>

---

**Problem 2:** Is this AND or OR logic?
> "A movie appears in 'Recommended' if it has a high rating OR a friend recommended it"

<details>
<summary>Answer</summary>

**OR** - Either condition is enough to recommend it. A movie with low rating but friend-recommended still shows up.
</details>

---

**Problem 3:** What could go wrong?
> You're writing code to get a user's email from their profile data

<details>
<summary>Things to consider</summary>

- The user data might not have an "email" key
- The email value might be None
- The entire user data might be empty
- You should use safe access methods
</details>

---

# 📗 PHASE 2: Python Foundations

## The Building Blocks

Everything in Python builds on these fundamentals. Make sure you're solid here.

---

## 2.1 Variables and Data Types

```
┌─────────────────────────────────────────────────────┐
│                   DATA TYPES                        │
├─────────────────────────────────────────────────────┤
│                                                     │
│  STRING (str)        TEXT                          │
│  "Hello"             "sam@email.com"                │
│                                                     │
│  INTEGER (int)       WHOLE NUMBERS                 │
│  42                  -7                 0          │
│                                                     │
│  FLOAT               DECIMAL NUMBERS               │
│  3.14                99.99             0.5         │
│                                                     │
│  BOOLEAN (bool)      TRUE OR FALSE                 │
│  True                False                         │
│                                                     │
│  NONE                NOTHING / MISSING             │
│  None                (represents absence)          │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**Key understanding:**
- `"True"` (string) is NOT the same as `True` (boolean)
- `None` is NOT the same as `0` or `""`
- Know what type your data is!

---

## 2.2 Conditionals: if / elif / else

```
┌─────────────────────────────────────────────────────┐
│              CONDITIONAL FLOW                       │
│                                                     │
│                    START                            │
│                      │                              │
│                      ▼                              │
│               ┌─────────────┐                       │
│               │ if condition│                       │
│               │   is True?  │                       │
│               └──────┬──────┘                       │
│                      │                              │
│          ┌───YES─────┴─────NO───┐                  │
│          │                      │                   │
│          ▼                      ▼                   │
│    ┌──────────┐          ┌─────────────┐           │
│    │ Do this  │          │elif condition│           │
│    └──────────┘          │   is True?  │           │
│                          └──────┬──────┘           │
│                                 │                   │
│                     ┌───YES─────┴─────NO───┐       │
│                     │                      │        │
│                     ▼                      ▼        │
│               ┌──────────┐          ┌──────────┐   │
│               │ Do this  │          │   else   │   │
│               └──────────┘          │ Do this  │   │
│                                     └──────────┘   │
└─────────────────────────────────────────────────────┘
```

**The pattern:**
```python
if condition1:
    # do this if condition1 is True
elif condition2:
    # do this if condition1 was False but condition2 is True
else:
    # do this if nothing above was True
```

**Common comparisons:**
- `==` equals
- `!=` not equals
- `>` greater than
- `<` less than
- `>=` greater than or equal
- `<=` less than or equal

---

## 2.3 Functions: The Input → Output Machine

```
┌─────────────────────────────────────────────────────┐
│                   FUNCTION                          │
│                                                     │
│        INPUT              PROCESS           OUTPUT  │
│     (parameters)         (your code)       (return) │
│                                                     │
│         │                    │                │     │
│         ▼                    ▼                ▼     │
│    ┌─────────┐        ┌───────────┐    ┌─────────┐ │
│    │  data   │───────▶│  Do stuff │───▶│ result  │ │
│    └─────────┘        └───────────┘    └─────────┘ │
│                                                     │
└─────────────────────────────────────────────────────┘

def function_name(input_parameter):
    # do something with input
    result = input_parameter + something
    return result
```

**Critical concept: return vs print**

```python
# This RETURNS a value (you can use it later)
def add(a, b):
    return a + b

result = add(5, 3)  # result is now 8

# This PRINTS but returns None
def add_broken(a, b):
    print(a + b)

result = add_broken(5, 3)  # prints 8, but result is None!
```

**Always ask:** Does my function **return** what it should?

---

## 2.4 Loops: Doing Things Repeatedly

### For Loops

```
┌─────────────────────────────────────────────────────┐
│                   FOR LOOP                          │
│                                                     │
│      items = [A, B, C, D]                          │
│                                                     │
│      ┌────────────────────────────────┐            │
│      │                                │            │
│      │   for item in items:           │            │
│      │       # do something           │            │
│      │                                │            │
│      └────────────────────────────────┘            │
│                                                     │
│      Loop 1: item = A  →  do something             │
│      Loop 2: item = B  →  do something             │
│      Loop 3: item = C  →  do something             │
│      Loop 4: item = D  →  do something             │
│      Done!                                          │
│                                                     │
└─────────────────────────────────────────────────────┘
```

### Common Loop Patterns

**Pattern 1: Accumulator (adding up)**
```python
total = 0
for number in numbers:
    total = total + number
# total now has the sum
```

**Pattern 2: Counter (counting things)**
```python
count = 0
for item in items:
    if some_condition:
        count = count + 1
# count now has how many matched
```

**Pattern 3: Builder (creating a new list)**
```python
new_list = []
for item in items:
    if some_condition:
        new_list.append(item)
# new_list has filtered items
```

---

## 2.5 Lists and Dictionaries

### Lists: Ordered Collections

```
┌─────────────────────────────────────────────────────┐
│                     LIST                            │
│                                                     │
│   Index:    0        1        2        3           │
│           ┌────┐   ┌────┐   ┌────┐   ┌────┐       │
│   items = │"a" │   │"b" │   │"c" │   │"d" │       │
│           └────┘   └────┘   └────┘   └────┘       │
│                                                     │
│   items[0]  →  "a"                                 │
│   items[2]  →  "c"                                 │
│   items[99] →  ERROR! (IndexError)                 │
│                                                     │
└─────────────────────────────────────────────────────┘
```

### Dictionaries: Key-Value Pairs

```
┌─────────────────────────────────────────────────────┐
│                  DICTIONARY                         │
│                                                     │
│   person = {                                        │
│       "name": "Sam",      ←── key: value           │
│       "age": 25,          ←── key: value           │
│       "city": "Boston"    ←── key: value           │
│   }                                                 │
│                                                     │
│   person["name"]   →  "Sam"                        │
│   person["age"]    →  25                           │
│   person["email"]  →  ERROR! (KeyError)            │
│                                                     │
└─────────────────────────────────────────────────────┘
```

---

## Phase 2 Practice Problems

**Problem 1:** What does this function return?
```python
def check_score(score):
    if score >= 90:
        return "A"
    elif score >= 80:
        return "B"
    else:
        return "C"

result = check_score(85)
```

<details>
<summary>Answer</summary>

Returns `"B"` - score is 85, which is not >= 90, but is >= 80
</details>

---

**Problem 2:** What does this print?
```python
numbers = [10, 20, 30, 40]
total = 0

for n in numbers:
    total = total + n

print(total)
```

<details>
<summary>Answer</summary>

Prints `100` (10 + 20 + 30 + 40 = 100)
</details>

---

**Problem 3:** What's wrong here?
```python
def get_double(x):
    print(x * 2)

result = get_double(5)
print(f"Result is: {result}")
```

<details>
<summary>Answer</summary>

The function prints `10` but **returns None**.
The second print shows `Result is: None`.
Fix: Change `print(x * 2)` to `return x * 2`
</details>

---

**Problem 4:** What does this return?
```python
data = {"name": "Alex", "score": 85}
value = data["email"]
```

<details>
<summary>Answer</summary>

**Crashes with KeyError!** The key "email" doesn't exist in the dictionary.
</details>

---

# 📙 PHASE 3: Applied Python

## Making Your Code Robust

This is where everything comes together. You'll learn to handle real-world messiness.

---

## 3.1 Safe Dictionary Access

**The problem:**

```
┌─────────────────────────────────────────────────────┐
│              THE DANGER OF [ ]                      │
│                                                     │
│   data = {"name": "Sam"}                           │
│                                                     │
│   data["name"]    →  "Sam"     ✓ Works             │
│   data["email"]   →  💥 CRASH! (KeyError)          │
│                                                     │
│   You can't always trust that keys exist!          │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**The solution: .get()**

```
┌─────────────────────────────────────────────────────┐
│              SAFE ACCESS WITH .get()                │
│                                                     │
│   data = {"name": "Sam"}                           │
│                                                     │
│   data.get("name")           →  "Sam"              │
│   data.get("email")          →  None (no crash!)   │
│   data.get("email", "N/A")   →  "N/A" (default)    │
│                                                     │
│                                                     │
│   SYNTAX:  dictionary.get(key, default_value)      │
│                                                     │
│   • If key exists: returns the value               │
│   • If key missing: returns default (or None)      │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**The pattern you'll use constantly:**

```python
def process_data(data):
    # Safely get values
    name = data.get("name")
    age = data.get("age")
    
    # Check if required data is missing
    if name is None or age is None:
        return {"error": "Missing data"}
    
    # Now safe to use name and age
    return {"name": name, "is_adult": age >= 18}
```

---

## 3.2 Checking for None

**Why this matters:**

```
┌─────────────────────────────────────────────────────┐
│               NONE CHECKING                         │
│                                                     │
│   value = data.get("key")                          │
│                                                     │
│   # This could be:                                  │
│   # - The actual value (if key exists)             │
│   # - None (if key doesn't exist)                  │
│                                                     │
│   # So always check before using:                   │
│                                                     │
│   if value is None:                                │
│       # handle the missing case                     │
│   else:                                             │
│       # safe to use value                           │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**Common patterns:**

```python
# Pattern 1: Return error if missing
value = data.get("required_field")
if value is None:
    return {"error": "Missing required field"}

# Pattern 2: Use default if missing
value = data.get("optional_field", "default_value")

# Pattern 3: Check multiple fields
name = data.get("name")
age = data.get("age")
if name is None or age is None:
    return {"error": "Incomplete data"}
```

---

## 3.3 Understanding JSON

```
┌─────────────────────────────────────────────────────┐
│                  JSON → PYTHON                      │
│                                                     │
│   JSON (text format)        Python (data types)    │
│   ──────────────────        ─────────────────────  │
│   { }                  →    dict                   │
│   [ ]                  →    list                   │
│   "string"             →    str                    │
│   123                  →    int                    │
│   12.5                 →    float                  │
│   true / false         →    True / False           │
│   null                 →    None                   │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**JSON data typically looks like:**
```json
{
    "name": "Sam",
    "age": 25,
    "active": true,
    "scores": [85, 92, 78]
}
```

**In Python, after parsing:**
```python
data = {
    "name": "Sam",
    "age": 25,
    "active": True,
    "scores": [85, 92, 78]
}
```

**Working with JSON in Python:**
```python
import json

# String → Dictionary
json_string = '{"name": "Sam", "age": 25}'
data = json.loads(json_string)

# Now data is a regular Python dictionary
print(data["name"])  # "Sam"
```

---

## 3.4 Basic Error Handling with try/except

```
┌─────────────────────────────────────────────────────┐
│              TRY / EXCEPT FLOW                      │
│                                                     │
│   try:                                              │
│       # Risky code goes here                        │
│       │                                             │
│       ▼                                             │
│   ┌─────────────────┐                              │
│   │ Does it work?   │                              │
│   └────────┬────────┘                              │
│            │                                        │
│     YES────┴────NO                                  │
│      │          │                                   │
│      ▼          ▼                                   │
│   Continue   except:                               │
│   normally      # Handle the error                 │
│                 # Don't crash                       │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**Common error types:**

| Error | When It Happens |
|-------|-----------------|
| `KeyError` | Dictionary key doesn't exist |
| `IndexError` | List index out of range |
| `TypeError` | Wrong type (e.g., can't add string + number) |
| `ValueError` | Right type but wrong value |
| `FileNotFoundError` | File doesn't exist |
| `ZeroDivisionError` | Dividing by zero |

**Example:**
```python
def safe_divide(a, b):
    try:
        return a / b
    except ZeroDivisionError:
        return "Cannot divide by zero"
```

---

## 3.5 Putting It All Together

**The complete pattern for handling external data:**

```
┌─────────────────────────────────────────────────────┐
│           ROBUST DATA HANDLING PATTERN              │
│                                                     │
│   1. GET DATA SAFELY                               │
│      └─▶ Use .get() instead of []                  │
│                                                     │
│   2. CHECK FOR MISSING DATA                        │
│      └─▶ if value is None: handle it              │
│                                                     │
│   3. PROCESS THE DATA                              │
│      └─▶ Now safe to use the values               │
│                                                     │
│   4. RETURN APPROPRIATE RESULT                     │
│      └─▶ Success case or error message            │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**Example putting it all together:**

```python
def process_user(user_data):
    # 1. Get data safely
    name = user_data.get("name")
    age = user_data.get("age")
    
    # 2. Check for missing data
    if name is None or age is None:
        return {"error": "Missing required fields"}
    
    # 3. Process the data
    is_adult = age >= 18
    
    # 4. Return appropriate result
    return {
        "name": name,
        "is_adult": is_adult
    }
```

---

## Phase 3 Practice Problems

**Problem 1:** What does this return?
```python
data = {"name": "Sam", "score": 85}
email = data.get("email", "none@example.com")
print(email)
```

<details>
<summary>Answer</summary>

Prints `none@example.com` - the key "email" doesn't exist, so the default is used.
</details>

---

**Problem 2:** What's wrong with this code?
```python
def get_status(user):
    name = user["name"]
    active = user["active"]
    
    if active:
        return f"{name} is active"
    else:
        return f"{name} is inactive"
```

<details>
<summary>Answer</summary>

Uses `[]` instead of `.get()` - will crash if "name" or "active" keys are missing.

**Fix:**
```python
def get_status(user):
    name = user.get("name")
    active = user.get("active")
    
    if name is None or active is None:
        return "Unknown status"
    
    if active:
        return f"{name} is active"
    else:
        return f"{name} is inactive"
```
</details>

---

**Problem 3:** Complete this function
```python
def is_premium(account):
    # Return True if account type is "premium"
    # Return False if account type is anything else
    # Return False if "type" key is missing
    # Use .get()
    pass
```

<details>
<summary>Answer</summary>

```python
def is_premium(account):
    account_type = account.get("type")
    return account_type == "premium"
```

Or more explicitly:
```python
def is_premium(account):
    account_type = account.get("type")
    if account_type is None:
        return False
    return account_type == "premium"
```
</details>

---

**Problem 4:** What does this print?
```python
items = [
    {"name": "apple", "price": 2},
    {"name": "banana"},
    {"name": "orange", "price": 3}
]

total = 0
for item in items:
    price = item.get("price", 0)
    total = total + price

print(total)
```

<details>
<summary>Answer</summary>

Prints `5` (2 + 0 + 3 = 5)

The banana has no price, so `.get("price", 0)` returns 0.
</details>

---

# ✅ SELF-ASSESSMENT CHECKLIST

Before your assessment, make sure you can do all of these:

## Phase 1: Thinking & Planning
- [ ] I can break a problem into logical steps
- [ ] I can explain the difference between AND and OR logic
- [ ] I can anticipate what might go wrong with data
- [ ] I can explain my approach before I code

## Phase 2: Python Foundations
- [ ] I know the basic data types (str, int, float, bool, None)
- [ ] I can write if/elif/else statements correctly
- [ ] I can write functions with parameters and return values
- [ ] I understand the difference between print and return
- [ ] I can write and trace for loops
- [ ] I can access list items by index
- [ ] I can access dictionary values by key

## Phase 3: Applied Python
- [ ] I use `.get()` to safely access dictionary keys
- [ ] I check for `None` before using values
- [ ] I can handle missing data gracefully
- [ ] I can return error dictionaries when things go wrong
- [ ] I understand how JSON becomes Python dictionaries
- [ ] I can trace code and predict what it outputs

---

# 🎯 FINAL TIPS FOR SUCCESS

## During the Assessment

### Part 1 (Verbal Planning)
- **Think out loud** - We want to hear your process
- **Break it into steps** - "First I'd... then I'd... finally I'd..."
- **Mention errors** - "This could go wrong if..."
- **Take a breath** - It's okay to pause and think

### Part 2 (Code or Debug)
- **Start with structure** - Write the def line first
- **Use .get()** - Safer than brackets
- **Check for None** - Before using values
- **Return something** - Don't forget the return!
- **Talk through it** - Explain what you're doing

### Part 3 (Trace)
- **Go line by line** - Don't skip ahead
- **Track variables** - What's the value at each step?
- **Follow the loop** - Step through each iteration
- **Say your answer clearly** - "It prints X because..."

## Common Mistakes to Avoid

| Mistake | Why It's Wrong | What To Do |
|---------|----------------|------------|
| Using `[]` on dictionaries | Crashes if key missing | Use `.get()` |
| Forgetting to check None | Causes errors later | Add `if value is None:` |
| Using print instead of return | Function returns None | Use `return` |
| `"True"` instead of `True` | String, not boolean | Remove quotes |
| No return in else branch | Returns None | Add return statement |

---

## 🌟 You've Got This!

**Remember:**
- This assessment covers what you've been learning all along
- You're not expected to be perfect
- Showing your thinking matters
- Partial credit exists - try everything
- We're here to see your growth

**You've learned so much. Now show us what you know!**

Good luck! 🚀
