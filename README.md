# ThreadForge

A web app to understand OS concepts like threads, processes, and deadlocks.

## Features

**Thread Simulator**
- Create processes and threads, watch them move through states (New → Ready → Running → Blocked → Terminated)
- Control scheduling yourself - step through it manually to see what actually happens
- See everything with color codes so you know what state each thread is in

**Two Classic Problems**
- **Producer-Consumer**: Set up producers and consumers, see how they share a buffer without stepping on each other
- **Dining Philosophers**: Watch the naive solution deadlock, then see how changing the order of fork requests fixes it

---

## Getting Started

**Online**:
```
https://haggaiyes.github.io/threadforge/
```

**Locally**: 
1. Download or clone the repo
2. Open `index.html` in your browser

---

## How to Use It

**Create processes** - Hit the button, name your process, add some threads

**Schedule threads** - Click "Admit" to move them from New to Ready, "Dispatch" to run them, "Preempt" to pause them, "Block" if they need to wait

**Run the examples** - Click on Philosophers or Producer-Consumer to see them in action. Hit Step to move forward one at a time. Watch the log to see what's happening.

**Save your setup** - Scenarios save to your browser, so you can reload them later

---

## Tech Stack

- HTML5 + CSS3 + Vanilla JavaScript
- Single file, no dependencies
- Works in any modern browser (Chrome, Firefox, Safari, Edge)
- Saves your scenarios to browser storage so they stick around

## Tested Against

- Simple thread lifecycle transitions
- Context switching and preemption
- The classic Dining Philosophers deadlock (naive version)
- Dining Philosophers with resource hierarchy (no deadlock)
- Producer-Consumer with bounded buffers
- Thread blocking and waking

## Notes

- Single core only (doesn't model multi-core stuff)
- Semaphores are simplified - it's a learning tool, not a kernel
- Everything is step-by-step and manual, no real concurrency happening under the hood
- Scenarios save to your browser, so clearing browser data will wipe them

---

Made in 2026
