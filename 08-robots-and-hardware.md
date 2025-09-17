# Chapter 8: Robots & Hardware (Physical Computing)

## What Makes a Robot a Robot?

A robot is a machine that can:
1. **Sense** its environment (sensors)
2. **Think** about what to do (processor/computer)
3. **Act** in the physical world (actuators/motors)

**Not Robots:** Washing machine (just follows a timer)
**Robots:** Roomba vacuum (senses walls, decides where to go, moves around)

## Robot Parts: The Building Blocks

### Sensors: Robot Senses
Just like you have senses, robots have sensors:

**Human → Robot**
- Eyes → Camera
- Ears → Microphone
- Touch → Pressure sensor
- Balance → Gyroscope
- Temperature → Thermometer

**Special Robot Sensors:**
- Ultrasonic: Uses sound waves to measure distance (like a bat!)
- Infrared: Detects heat
- Light sensor: Measures brightness
- Motion detector: Senses movement

### Actuators: Robot Muscles
These make robots move:
- **Motors:** Make wheels turn or arms move
- **Servos:** Motors that move to specific positions
- **LEDs:** Lights for communication
- **Speakers:** Make sounds or talk
- **Pumps:** Move liquids or air

### The Brain: Microcontrollers
Small computers that control robots:
- Arduino: Great for beginners
- Raspberry Pi: More powerful, runs like a mini computer
- micro:bit: Designed for education

## How Robots Make Decisions

### Simple Robot Logic
```python
# Line-following robot
while True:
    if sensor_sees_black:
        turn_left_slightly()
    else:
        turn_right_slightly()
    move_forward()
```

### More Complex Decisions
```python
# Obstacle-avoiding robot
distance = ultrasonic_sensor.measure()
if distance < 10cm:
    stop()
    look_left_distance = check_left()
    look_right_distance = check_right()

    if look_left_distance > look_right_distance:
        turn_left()
    else:
        turn_right()
else:
    move_forward()
```

## Types of Robots

### Helper Robots
- **Roomba:** Vacuums your floor
- **Robot arms:** Build cars in factories
- **Delivery robots:** Bring packages to your door
- **Medical robots:** Help with surgery

### Explorer Robots
- **Mars rovers:** Explore other planets
- **Underwater robots:** Study the ocean
- **Drone:** Fly and take pictures
- **Search and rescue:** Find people after disasters

### Social Robots
- **Alexa/Siri:** Voice assistants
- **Pepper:** Humanoid robot that recognizes emotions
- **Robot pets:** Companions that respond to touch

## Build Your Own Simple "Robot"

### Paper Circuit Greeting Card
**Materials:**
- LED light
- Coin battery
- Copper tape
- Paper

**Steps:**
1. Draw a circuit path
2. Lay copper tape on the path
3. Add LED and battery
4. When circuit closes, LED lights up!

### Bristlebot: Tiny Vibrating Robot
**Materials:**
- Toothbrush head
- Small motor
- Battery
- Rubber band

The vibrating motor makes the brush "walk"!

## Programming Robot Behavior

### State Machines: Robot Moods
Robots can have different "states" or moods:

```python
robot_state = "EXPLORING"

if robot_state == "EXPLORING":
    move_forward()
    if obstacle_detected:
        robot_state = "AVOIDING"

elif robot_state == "AVOIDING":
    turn_right()
    if path_clear:
        robot_state = "EXPLORING"

elif robot_state == "LOW_BATTERY":
    return_to_charger()
```

## Smart Homes and IoT

IoT = Internet of Things (everyday objects connected to the internet)

**Smart Home Examples:**
- Lights that turn on when you enter
- Thermostat that learns your schedule
- Doorbell with camera
- Fridge that tracks your groceries

**How It Works:**
1. Sensor detects something (motion, temperature, etc.)
2. Sends signal to computer/phone
3. You or the system makes a decision
4. Device takes action

## Robot Ethics: Important Questions

- Should robots make decisions about people's lives?
- What if a self-driving car has to choose who to protect?
- Should robots look like humans?
- Who's responsible if a robot makes a mistake?

## Fun Activity: Design Your Dream Robot

Draw and describe your robot:
1. **What does it do?**
2. **What sensors does it need?**
3. **How does it move?**
4. **What problems does it solve?**
5. **Write pseudocode for its main behavior**

Example: Pet-Feeding Robot
- Sensor: Clock (time), weight sensor (food bowl)
- Actuator: Motor to dispense food
- Logic: IF time == 6PM AND bowl_weight < 50g THEN dispense_food()

## The Future of Robotics

### Coming Soon
- Robots that learn from experience
- Soft robots (made of flexible materials)
- Swarm robots (many small robots working together)
- Nano-robots (tiny robots for medicine)

### Careers in Robotics
- Robotics Engineer
- AI Programmer
- Mechanical Designer
- Robot Operator
- Ethics Researcher

## Think About It

- What tasks would you want a robot to do for you?
- What tasks should humans always do themselves?
- How would you teach a robot to be gentle?

Next chapter: Let's explore the fascinating world of AI and machine learning!