Sorting Algorithm Visualizer
Overview

Sorting Algorithm Visualizer is an interactive web application built to demonstrate how classic sorting algorithms operate step-by-step.

The goal of this project is to strengthen algorithmic intuition by visually representing comparisons, swaps, and state transitions in real time using a modular rendering architecture.

This project focuses specifically on sorting algorithm execution and visualization through a structured trace-driven animation system.

Problem It Solves

Many learners understand sorting algorithms conceptually but struggle to visualize:

How elements move over time

How recursive algorithms transform arrays

Why time complexities differ

What happens internally during swaps and partitions

This project bridges that gap by providing a deterministic, replayable animation pipeline.

Implemented Algorithms

Bubble Sort — O(n²)

Selection Sort — O(n²)

Insertion Sort — O(n²)

Merge Sort — O(n log n)

Quick Sort — O(n log n average)

Heap Sort — O(n log n)

Each algorithm is executed independently from the visualization layer.

Architecture

The application follows a modular design pattern separating execution logic from rendering logic.

1. Algorithm Layer

Contains pure sorting implementations

Emits structured trace events instead of directly updating UI

Maintains clean separation of concerns

2. Tracer Layer

Captures algorithm execution steps

Stores state snapshots

Enables deterministic replay

3. Renderer Layer

Consumes tracer state

Responsible for visual output

Updates UI based on controlled animation timing

4. Player / State Management

Controls play, pause, step-forward functionality

Adjusts animation speed

Manages visualization progress

This separation ensures scalability and easier extension of new algorithms.

Key Engineering Decisions

Decoupled algorithm execution from UI rendering

Centralized animation control for deterministic playback

Modular component-based structure

Reusable tracer abstraction for different data structures

State-driven rendering for consistency

Tech Stack

React

JavaScript (ES6+)

SCSS Modules

Modular component architecture

Event-driven animation pipeline
