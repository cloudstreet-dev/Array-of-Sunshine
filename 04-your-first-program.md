# Chapter 4: Your First Program (Introduction to Coding)

## What is a Programming Language?

Just like people speak different languages (English, Spanish, Chinese), we can talk to computers using different programming languages!

Popular languages include:
- **Scratch:** Uses colorful blocks (great for beginners!)
- **Python:** Easy to read, like writing in English
- **JavaScript:** Makes websites interactive
- **Java:** Used in Minecraft!

## Pseudocode: Planning Your Program

Before coding, programmers often write "pseudocode" - fake code that explains what they want to do:

```
START
  Ask user for their name
  Store name in variable
  Say "Hello" + name
  Ask "How old are you?"
  Store age in variable
  Calculate birthYear = 2024 - age
  Say "You were born around " + birthYear
END
```

## Your First Real Program Ideas

### Program 1: The Greeting Bot
```python
name = input("What's your name? ")
print("Hello, " + name + "!")
print("Nice to meet you!")
```

### Program 2: The Calculator
```python
number1 = 10
number2 = 5
sum = number1 + number2
print("10 + 5 equals " + sum)
```

### Program 3: The Decision Maker
```python
weather = "sunny"
if weather == "sunny":
    print("Let's go to the park!")
else:
    print("Let's stay inside and play games!")
```

## Common Programming Concepts

**Comments:** Notes for humans (computers ignore them)
```python
# This is a comment - it helps explain the code
playerScore = 0  # Starting score
```

**Functions:** Reusable chunks of code
```python
def sayHello():
    print("Hello!")
    print("How are you?")

# Use the function
sayHello()  # This runs the function
```

**Events:** Things that trigger code
- Click a button → Run some code
- Press a key → Make character jump
- Timer ends → Game over

## Scratch: Visual Programming

If you have access to Scratch (scratch.mit.edu), try this:

1. **Make a sprite move:**
   - When [green flag] clicked
   - Move (10) steps
   - Turn (15) degrees
   - Repeat

2. **Make a sprite talk:**
   - When [space] key pressed
   - Say "Hello!" for (2) seconds

3. **Simple game:**
   - When [green flag] clicked
   - Forever:
     - Point towards (mouse pointer)
     - Move (3) steps

## Common Coding Mistakes (It's OK to Make Them!)

1. **Typos:** Computers are picky about spelling!
   - `print` ✓
   - `primt` ✗

2. **Forgetting quotation marks:**
   - `name = "Alex"` ✓
   - `name = Alex` ✗ (computer thinks Alex is a variable)

3. **Wrong order:**
   - Must create variable before using it
   - Must define function before calling it

## Fun Activity: Code Without a Computer!

Create a "program" for a dance:

```
START DANCE
  Repeat 2 times:
    Step right
    Step left
    Clap hands

  If music is fast:
    Jump 3 times
  Else:
    Spin around once

  Repeat 4 times:
    Wave arms

  Strike a pose
END DANCE
```

Now perform your programmed dance!

## Challenge: Design a Simple Game

On paper, design a simple game:
1. What's the goal?
2. What are the rules?
3. How do you win?
4. What happens when you lose?

Write the pseudocode for your game!

## Think About It

- What would you like to create with code?
- Why do you think there are so many programming languages?
- What's the difference between telling a friend what to do vs. telling a computer?

Next chapter: Let's explore how the internet works and how computers talk to each other!