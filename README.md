# Final-Year-Project---CogniFarm
AI-powered cognitive training mobile game with adaptive difficulty using Q-Learning and personalised reminders using Thompson Sampling.

# CogniFarm

AI-powered cognitive training mobile game that personalizes gameplay difficulty and notification timing using Reinforcement Learning.

---

## Overview

CogniFarm is a mobile cognitive training application developed as my Final Year Project at Nanyang Technological University.

The application combines gamified cognitive exercises with Reinforcement Learning to create a personalised training experience. Instead of using fixed difficulty levels or scheduled reminders, CogniFarm continuously adapts to each player's performance and engagement patterns to encourage user adherence and engagement.

The project integrates adaptive gameplay, intelligent notification scheduling, cloud data storage, and analytics into a complete end-to-end mobile application.

---

## Key Features

### Adaptive Difficulty using Q-Learning

The game dynamically adjusts its difficulty based on each player's:

* Accuracy
* Response time
* Current difficulty level

A tabular Q-Learning agent learns the optimal difficulty adjustments over time to keep players within an optimal challenge zone, improving engagement while avoiding frustration.

---

### Personalized Notification Timing using Thompson Sampling

Rather than sending reminders at a fixed time every day, CogniFarm learns:

* when each player is most likely to return,
* what reminder strategy works best,
* and continuously updates its policy based on previous engagement.

The reminder system combines:

* Thompson Sampling
* Bayesian updating
* Firebase Cloud Functions
* Firebase Cloud Messaging (FCM)

to deliver personalised notifications.

---

### Cognitive Training Mini Games

#### Harvesting Memory

A sequence memory game that trains working memory by requiring players to remember and reproduce increasingly difficult visual sequences.

#### Planting Seeds

A card matching game that improves concentration, pattern recognition, and short-term memory through progressively harder matching challenges.

---

## Tech Stack

### Game Development

* Unity
* C#

### Artificial Intelligence

* Reinforcement Learning (Q-Learning)
* Thompson Sampling

### Backend

* Firebase Firestore
* Firebase Cloud Functions
* Firebase Cloud Messaging (FCM)
* Cloud Scheduler

### Data & Analytics

* Firestore
* JSON persistence
* Player session analytics

---

## System Architecture

The application consists of several integrated components:

* Unity mobile application
* Adaptive Q-Learning engine
* Thompson Sampling notification engine
* Firebase backend
* Firestore database
* Cloud Functions for reminder scheduling
* Firebase Cloud Messaging for push notifications

---

## Reinforcement Learning

### Adaptive Difficulty

The Q-Learning agent models gameplay using:

* Performance level
* Response time
* Current difficulty

Each game session updates the Q-table, allowing the system to personalise future gameplay for each player.

Key characteristics include:

* 60-state environment
* 3 possible actions
* Reward function based on player performance and engagement
* Persistent learning across sessions

---

### Personalised Reminder System

The reminder engine uses Thompson Sampling to optimise notification timing.

Instead of relying on manually defined schedules, the agent continuously balances exploration and exploitation to identify the most effective reminder strategy for each player.

The system considers:

* Time of day
* Days since last session
* Previous reminder response
* Current activity streak

---

## Data Storage

Player information is stored securely using Firebase Firestore.

The system records:

* Gameplay sessions
* Scores
* Accuracy
* Response times
* Difficulty progression
* Reminder interactions
* Player engagement statistics

These records are used to personalise future gameplay and notification behaviour.

---

## Project Highlights

* AI-powered adaptive gameplay
* Personalized reminder scheduling
* Reinforcement Learning with Q-Learning
* Thompson Sampling for notification optimisation
* Firebase cloud backend
* End-to-end mobile application development
* Cross-platform Unity application
