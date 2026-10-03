# Printer Job Management System

A web app that shows how a **queue** works, using a printer as the real-world example.



## DSA concept: Queue (FIFO)

Print jobs must be handled in the order they arrive, so the first job in is the first job out. The queue is built from scratch with a **singly linked list** that keeps both a `head` (front) and a `tail` (rear) pointer.

| Operation | What it does in the app | Time |
|-----------|-------------------------|------|
| `enqueue` | Adds a new job at the rear | O(1) |
| `dequeue` | Sends the front job to the printer | O(1) |
| `peek`    | Shows the next job without removing it | O(1) |
| `clear`   | Cancels all waiting jobs | O(1) |

Because the list tracks the tail, adding a job never has to walk the whole list.

## Features
- Add jobs with a document name and page count
- Print the next job with a live progress bar
- Front and rear labels, queue size, and printed count
- Operation log that records every enqueue, dequeue, and peek

## Run it
Open `index.html` in a browser. No install or build step.

## Tech
HTML, CSS, and vanilla JavaScript in a single file.
