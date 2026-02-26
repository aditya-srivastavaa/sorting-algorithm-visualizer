🚀 Sorting Algorithm Visualizer

An interactive React-based web application that demonstrates how classic sorting algorithms operate step-by-step through a deterministic, trace-driven animation pipeline.

🎯 Why This Project?

Understanding sorting algorithms conceptually is easy.
Understanding how elements actually move during execution is not.

This project visually represents:

🔁 Comparisons

🔄 Swaps

📊 State transitions

⚡ Execution flow

It bridges the gap between theory and execution.

🧠 Implemented Algorithms
Algorithm	Best Case	Average Case	Worst Case
Bubble Sort	O(n)	O(n²)	O(n²)
Selection Sort	O(n²)	O(n²)	O(n²)
Insertion Sort	O(n)	O(n²)	O(n²)
Merge Sort	O(n log n)	O(n log n)	O(n log n)
Quick Sort	O(n log n)	O(n log n)	O(n²)
Heap Sort	O(n log n)	O(n log n)	O(n log n)

Each algorithm executes independently from the visualization engine.

🏗 Architecture

The application is built around strict separation of concerns.

1️⃣ Algorithm Layer

Pure sorting logic

Emits structured trace events

No direct UI manipulation

2️⃣ Tracer Layer

Records execution steps

Stores intermediate states

Enables deterministic replay

3️⃣ Renderer Layer

Consumes tracer state

Updates visual components

React-driven UI rendering

4️⃣ Player / State Control

Controls play, pause, step-forward

Manages animation timing

Handles speed adjustment

This modular architecture ensures extensibility and maintainability.

⚙️ Tech Stack

React

JavaScript (ES6+)

SCSS Modules

Modular component design

State-driven animation system

🔬 Engineering Focus

Decoupling execution logic from visualization

Deterministic animation playback

Modular component structure

Extensible algorithm integration

Clean state-driven rendering
