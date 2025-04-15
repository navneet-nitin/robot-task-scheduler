# robot-task-scheduler
# 🤖 RoboX – Task Scheduling for the Robotic Assistant

**RoboX** is a lightweight Java logic simulator that calculates how many sequential tasks a robotic assistant can perform within a limited amount of time. Each task takes progressively more time to complete — Task 1 takes 1 hour, Task 2 takes 2 hours, and so on.

✅ No Java installation required — the project is deployed online!

👉 **[Try it Live](https://navneet-nitin.github.io/robot-task-scheduler/)**

---

## 🚩 Problem Statement

In real-world automation (like home robots, warehouse bots, or assembly line machines), time and energy are limited. Tasks tend to become more time-consuming as robots operate continuously.

This project solves the key scheduling problem:

> **"Given a fixed amount of available time, how many consecutive tasks can the robot complete?"**

---

## 💡 Real-Life Relevance

- **Warehouse & Delivery Robots**: Task optimization before battery drain  
- **Cleaning Robots**: How many rooms can be cleaned in a fixed time?  
- **Production Lines**: How many jobs can a robotic arm complete before maintenance or shift-end?  
- **AI Assistants**: Planning time-constrained tasks that grow in complexity

---

## ⚙️ How It Works

1. The user enters the total number of available hours.
2. The program checks how many tasks can be completed, given that:
   - Task 1 = 1 hr
   - Task 2 = 2 hrs
   - ...
   - Task `k` = `k` hrs
3. Once total time used exceeds the available hours, the task count stops.

### 🔍 Behind the Scenes:
This follows the triangular number logic:  
`Total time = 1 + 2 + 3 + ... + k = k(k+1)/2`  
We find the maximum `k` such that the sum ≤ total time.

---

## 💻 Live Demo

Click below to use the simulator directly in your browser (no downloads needed):  
👉 **[https://navneet-nitin.github.io/robot-task-scheduler/](https://navneet-nitin.github.io/robot-task-scheduler/)**

---

## 🛠️ Built With

- **HTML + JavaScript** (for browser execution)
- **Java logic simulated through JS**
- **Deployed via GitHub Pages**

---


