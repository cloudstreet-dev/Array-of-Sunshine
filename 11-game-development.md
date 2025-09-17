# Chapter 11: Game Development (Making Your Own Games!)

## What Makes a Game a Game?

Every game has:
- **Goal:** What you're trying to achieve
- **Rules:** What you can and can't do
- **Feedback:** Knowing how you're doing
- **Challenge:** Not too easy, not too hard

## The Game Development Process

### 1. Idea & Design
Before coding, plan your game:
- What's the story?
- Who's the main character?
- What's the goal?
- What makes it fun?

### 2. Prototype
Make a super simple version:
- Use paper and pencil first!
- Test the basic idea
- Is it fun?

### 3. Development
Build the actual game:
- Start simple
- Add features one at a time
- Test constantly

### 4. Testing & Polish
- Find bugs
- Balance difficulty
- Add sound and music
- Make it look good

## Core Game Components

### Game Loop: The Heart of Every Game
```python
while game_running:
    handle_input()      # Check keyboard/mouse
    update_game()       # Move things, check collisions
    draw_everything()   # Show on screen
    wait(1/60 second)   # 60 frames per second
```

### Sprites: Your Game Characters
Sprites are images that move around:
- Player character
- Enemies
- Power-ups
- Obstacles

### Collision Detection
Checking when things touch:
```python
if player.touches(enemy):
    player.lose_life()
if player.touches(coin):
    score += 10
```

## Game Physics

### Gravity
```python
player.velocity_y += gravity
player.y += player.velocity_y

if player.touches_ground():
    player.velocity_y = 0
```

### Jumping
```python
if spacebar_pressed and player.on_ground:
    player.velocity_y = -jump_power
```

### Friction
```python
player.velocity_x *= 0.9  # Slowly stops moving
```

## Types of Games You Can Make

### Platformer
- Run and jump
- Collect items
- Avoid enemies
- Examples: Mario, Sonic

### Puzzle
- Solve problems
- Think ahead
- Examples: Tetris, Candy Crush

### Adventure
- Explore worlds
- Solve mysteries
- Examples: Zelda, Pokemon

### Endless Runner
- Keep going as long as possible
- Gets harder over time
- Examples: Temple Run, Flappy Bird

## Your First Game: Catch the Falling Stars

```python
# Pseudocode for simple game
score = 0
player_x = screen_width / 2
stars = []

while game_running:
    # Move player with arrow keys
    if left_arrow:
        player_x -= 5
    if right_arrow:
        player_x += 5

    # Create new stars
    if random() < 0.02:  # 2% chance each frame
        new_star = create_star(random_x_position, top_of_screen)
        stars.add(new_star)

    # Move stars down
    for star in stars:
        star.y += 3

        # Check if caught
        if star.touches(player):
            score += 1
            remove(star)

        # Remove if off screen
        if star.y > screen_height:
            remove(star)

    # Draw everything
    draw_player(player_x)
    draw_stars(stars)
    draw_score(score)
```

## Game Design Principles

### Difficulty Curve
Start easy, get gradually harder:
- Level 1: Learn controls
- Level 2: Easy challenge
- Level 3: New mechanic
- Level 4: Combine skills

### Risk vs Reward
Give players interesting choices:
- Big coin worth 10 points but dangerous to get
- Safe path = slow, Dangerous path = fast

### Feedback
Let players know what's happening:
- Sound when collecting items
- Screen shake when hit
- Particles when jumping
- Score pop-ups

## Game Art & Animation

### Pixel Art Basics
Start with small sprites (16x16 or 32x32 pixels):
- Use limited colors
- Every pixel matters
- Animate with 3-4 frames

### Animation Cycles
**Walk Cycle:** 4 frames
1. Right foot forward
2. Passing position
3. Left foot forward
4. Passing position

**Idle Animation:** 2 frames
1. Normal standing
2. Slight breathing motion

## Sound in Games

### Types of Game Audio
- **Music:** Sets the mood
- **Sound Effects:** Actions and feedback
- **Ambient Sound:** Background atmosphere
- **Voice:** Character dialogue

### Creating Simple Sounds
Use online tools to generate:
- Beeps and boops for retro games
- Whoosh sounds for jumping
- Ding for collecting items

## Level Design

### Good Level Design
- Teaches without words
- Gradually introduces concepts
- Has a rhythm (action, rest, action)
- Rewards exploration

### Paper Level Design
Draw your level first:
- Start point
- End goal
- Enemies
- Power-ups
- Secret areas

## Game Balance

### Making It Fair
- Playtest with different people
- Not too easy (boring)
- Not too hard (frustrating)
- Multiple ways to win

### Economy Balance
If your game has coins/points:
- How much do things cost?
- How fast do players earn?
- What can they buy?

## Fun Activity: Design a Board Game

Before coding, make a physical game:
1. Use paper, dice, and markers
2. Create simple rules
3. Test with family
4. Adjust rules based on feedback
5. This is exactly how video game design works!

## Game Development Tools

### For Beginners
- **Scratch:** Drag-and-drop game making
- **MakeCode Arcade:** Block-based arcade games
- **Construct 3:** Visual game development

### For Next Level
- **Godot:** Free, powerful, beginner-friendly
- **Unity:** Professional tool (Minecraft was partly made with this!)
- **Pico-8:** Retro game maker

## Publishing Your Game

- Share with friends and family
- Upload to Scratch community
- Put on itch.io (indie game site)
- Get feedback and improve!

## Game Development Careers

- Game Designer (creates ideas and rules)
- Programmer (writes the code)
- Artist (creates graphics)
- Sound Designer (makes music and effects)
- Level Designer (creates worlds)
- Game Tester (finds bugs)

## Think About It

- What makes your favorite game fun?
- How would you improve a game you play?
- What story would you tell in a game?

Next chapter: Let's explore how technology helps scientists and engineers!