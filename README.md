# EDS Class Computer Science Teaching Portfolio

Welcome to my teaching portfolio for CS education. The following repo will include tasks and assignments that will document my learning process of teaching CS!

---

## Peer-graded Assignment: Animal Parade (Scratch Act 1) - Code Explanation

### Loops & Repetition: Kangaroo, Grasshopper, and Bee
- **Project:** Loops: Animal Parade (UCSD Version)
- **Tool:** Scratch (MIT)
- **Video Walkthrough:** https://www.loom.com/share/5fb798a78fb845fc8843c93e83284b40

#### Program & Concept Description
This project explores program creation knowledge through the **TIPP&SEE** framework, contrasting repeated imperative code sequences with structured `repeat` loops. The Quest implementation coordinates three sprites:
- **Kangaroo:** Executes synchronized arc jumps forward using a `repeat (4)` loop, adjusting $x$ and $y$ offsets while toggling between jumping and crouching costumes.
- **Grasshopper:** Leverages a `repeat (5)` loop with short wait timings to simulate rapid forward hops across the lawn.
- **Bee:** Follows a circular flight path when clicked, using a `repeat (24)` loop that moves forward and turns right by $15^\circ$ ($24 \times 15^\circ = 360^\circ$) while continuously updating costumes to animate wing flaps.

---

## Peer-graded Assignment: Show What You Know: Explain Your Program

### Snap! Spirograph Demonstration
- **Project:** Colorful Spirograph in Motion
- **Tool:** Snap! (UC Berkeley)
- **Video Walkthrough:** https://www.loom.com/share/d3ebf2c45cfa4a97b206bf79a8061452

#### Program Description
This program generates an interactive rainbow geometric spirograph using motion, rotation angles, and dynamic pen drawing blocks in Snap!. It demonstrates coordinate resets, dynamic pen colors, and looping rotation algorithms.

---

## Peer-graded Assignment: Document Understanding with a Video Explanation (Repeats)

### Snap! WP_Repeats Breakdancer Demonstration
- **Project:** Breakdancer Routine with Iteration (WP_Repeats)
- **Tool:** Snap! (UC Berkeley)
- **Video Walkthrough:** https://www.loom.com/share/44dab3eb4e4248308c07320e30f87372

#### Program & Concept Description
This video demonstration explains how repetition constructs consolidate repetitive motion routines and structure program flow:
- **The purpose of my program is** to animate a breakdancer performing a timed, continuous dance sequence across the stage using sequential costume swaps and coordinated delays.
- **My code works by using repeats in this part to** iterate over the primary animation routine, toggling between `breakdancer1 c` and `breakdancer1 a` costumes with paired wait blocks to produce fluid visual movement without manual block duplication.
- **If I were to change this repeat like this** by modifying the loop iteration count or adjusting the delay between costume switches, **the program would run differently** by either shortening the overall duration of the dance performance or altering the tempo and visual cadence of the sprite's movement on stage.

---

## Peer-graded Assignment: Document Understanding with a Video Explanation (Nested Repeats)

### Snap! Nested Repeats Mouse Octagon Demonstration
- **Project:** Nested Repeats: Mouse Octagon Drawing
- **Tool:** Snap! (UC Berkeley)
- **Video Walkthrough:** https://www.loom.com/share/ef8e2687bc59405aacfe05b9d8a21cf6

#### Program & Concept Description
This video demonstration documents how nested iteration models multi-level geometric procedures through nested control structures:
- **The purpose of my program is** to guide a mouse sprite through an automated dialogue sequence and systematically trace an 8-sided regular octagon on the stage.
- **My code works by using nested repeats in this part to** coordinate the outer turning geometry with the inner side translation:
  - **Outer Loop (`repeat 8`):** Handles the eight vertices of the polygon by rotating the mouse by $45^\circ$ ($360^\circ / 8 = 45^\circ$), displaying a `"Squeak!"` speech bubble, and pausing before beginning each edge.
  - **Inner Nested Loop (`repeat 4`):** Subdivides each side of the octagon into four discrete movements of 20 steps with 0.5-second pauses, producing an 80-step edge length before yielding control back to the outer rotation block.
- **If I were to change this nested repeat like this** by reducing the outer `repeat` count from 8 to 6, updating the turn angle from $45^\circ$ to $60^\circ$ ($360^\circ / 6 = 60^\circ$), and modifying the inner `repeat` from 4 to 2, **the program would run differently** by drawing a smaller 6-sided regular hexagon with 40-step edges instead of a full octagon.
