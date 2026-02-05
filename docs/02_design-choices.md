# Design Choices

This project prioritizes emotional safety and non-intrusive interaction over technical complexity or performance.

### Screen-based Interaction
Instead of motors or locomotion, a screen-based expressive face was chosen to convey presence and emotion. This reduced mechanical complexity while allowing rich, subtle feedback through animations.
### One-directional Care
The robot offers reminders, affirmations, and check-ins without requiring user responses. This avoids creating pressure, obligation, or emotional dependency.
### Physical Restraint
The robot is designed to be desk-sized, quiet by default, and easy to store. A silent mode is included to respect study and rest environments.

## Feature Lock (v1)
This project intentionally limits scope to prioritize emotional safety, feasibility, and completion within five months. Features not listed here are explicitly excluded from v1.

### 1. Core Interaction Features: define the robot’s personality.
**Motion-based awareness (IMU)**
- Picked up → wakes up (eyes open, soft sound)
- Tilted → reacts gently (expression change)
- Put down → settles / rests

Purpose: feels “alive” without demanding attention
 
**Touch interaction (petting)**
- Capacitive touch on the top
- Petting → expression softens / happy reaction
- No negative reactions

Rule: touch only gives positive or neutral feedback

**Expressive screen face**
- Simple eyes + mouth
- Limited number of expressions (see below)
- No complex animation systems

**Audio feedback (built-in speaker)**
- Soft voice lines only
- No loud alerts
- Volume capped
- Silent mode overrides all audio

### 2. Emotional Support Features (LOCKED): These are the reason the robot exists.
**Gentle reminders**
- Eat
- Rest
- Reduce smoking (phrased gently)

Rules:
- No guilt,
- No repetition spam,
- Can be muted

**Affirmations**
Examples:
“I’m proud of you.”,
“You’re doing your best.”,
“I’m here.”

Randomized, infrequent, never triggered by failure.

**Occasional check-in**
Passive questions like:
“Have you eaten today?”

No required response,
No tracking behavior

**Countdown to next meeting**
- Displays days remaining
- Optional view
- Emotional anchor, not a timer

### 3. Physical & System Constraints (LOCKED): These protect feasibility.
**Form factor**
- Desk-sized
- Fits battery + board + speaker
- Portable
- Carrying case / gantungan compatible

**Silent mode**
- Fully disables audio
- Visual-only reactions remain

**No motors**
- No wheels
- No arms
- No actuators

This is a design decision, not a limitation.

### 4. Explicitly NOT in v1 (VERY IMPORTANT)
❌ Speech recognition / conversation
❌ Emotion detection
❌ Mobile app
❌ Internet dependency
❌ Camera
❌ Cloud / AI chatbot
❌ Complex animations
❌ Multiple touch zones

These go into “What I’d Improve”, not v1.

### 5. Expression Set (LOCKED & LIMITED)
Max 6 states:
- Sleeping
- Awake / Neutral
- Happy (petting)
- Concerned (reminder)
- Proud / Affirmation
- Settled / Calm

### 6. Hardware Assumptions (LOCKED)
- ESP32-S3 Touch LCD 1.46" (protective glass)
- Built-in IMU
- Built-in speaker
- Capacitive touch via screen
- Single Li-Po battery
- USB charging

No extra boards unless absolutely required.
