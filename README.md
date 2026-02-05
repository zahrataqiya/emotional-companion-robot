# emotional-companion-robot
*A human-centered robotics project*

## Overview
This project explores how a small, non-intrusive robot can provide gentle emotional support through quiet presence, reminders, and affirmations. Rather than focusing on movement or performance, the design prioritizes emotional safety, restraint, and everyday usability.

The robot is designed as a desk-sized companion for a busy engineering student, offering soft check-ins (eat, rest), affirmations, and subtle reactions to touch and motion. This project aims to demonstrate how embedded systems and mechanical design can be applied to real human problems, even in small, personal contexts.

## Motivation
I wanted every project I build to matter to someone or something, no matter how small the impact. This project was inspired by a close friend struggling with mental health, as well as by assistive technology projects that show how simple systems can meaningfully improve quality of life.

Instead of designing a robot that demands attention or interaction, this project focuses on presence without pressure.

## Core Features
- Screen-based expressive face (“micro-life” design)
- Gentle reminders (eat, rest, reduce smoking)
- Affirmations and supportive audio feedback
- Touch interaction (petting changes expression)
- Motion-based interaction (pick up, tilt, put down)
- Countdown display until next meeting
- Silent mode for study environments
- Desk-sized, portable form factor

## Design Philosophy
- Non-intrusive: The robot never demands interaction.
- Emotionally safe: No guilt-based reminders or dependency.
- Restrained complexity: Features are added only if they improve user experience.
- Human-centered: Engineering decisions are guided by real emotional needs.

## Hardware Overview
- ESP32-S3 round display development board (1.46", 412×412)
- Built-in speaker and microphone
- Accelerometer and gyroscope
- Capacitive touch input (for petting interaction)
- Rechargeable Li-Po battery
- Custom 3D-printed enclosure

## Repository Structure
```cpp
├── docs/              # Design documentation
│   ├── problem-statement.md
│   ├── design-choices.md
│   ├── failures.md
│   └── improvements.md
├── hardware/          # CAD, schematics, and physical design
├── firmware/          # ESP32-S3 code
├── media/             # Images and demo videos
└── devlog.md          # Weekly development notes
```

## What This Project Is (and Isn’t)
- ✅ A study in human-centered robotics and interaction design
- ✅ A personal but technically grounded engineering project
- ❌ Not a therapeutic or medical device
- ❌ Not intended to replace human support

## Status
Currently in active development.
Progress updates and short demos will be shared on TikTok (linked in profile).
