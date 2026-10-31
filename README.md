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

---

## Peer-graded Assignment: Document Understanding with a Video Explanation (Events)

### Snap! Monkey and Falling Banana Demonstration
- **Project:** Events & Inter-Sprite Communication: Monkey Banana Catch
- **Tool:** Snap! (UC Berkeley)
- **Video Walkthrough:** https://www.loom.com/share/6c069ef234ec40da9bccea6b55240c12

#### Program & Concept Description
This demonstration highlights how event-driven programming and message broadcasts coordinate decoupled sprites in an interactive environment:
- **The purpose of my program is** to operate an interactive catching game where a user controls a monkey along the ground using keyboard events to catch falling bananas before they touch the grass.
- **My code works by using events in this part to** orchestrate player control, collision sensing, and multi-sprite communication:
  - **Key-Press Events:** The monkey uses `when [right arrow] key pressed` and `when [left arrow] key pressed` event listeners to displace horizontal position incrementally (+10 / -10 steps).
  - **Conditional Event Triggers:** Predicate hat blocks (`when touching [banana]?` on the monkey and `when touching [green]?` on the banana) trigger immediately upon physical overlap without manual polling inside an imperative loop.
  - **Broadcast Signaling:** Inter-sprite messaging via `broadcast [resetBanana]` and `broadcast [missedBanana]` synchronizes state changes—relocating the falling fruit to the top of the stage and signaling the monkey sprite to trigger reactive speech bubbles.
- **If I were to change this event system like this** by altering the vertical velocity inside the banana's loop from `change y by -25` to `change y by -10` and modifying the tick delay, **the program would run differently** by reducing gravitational falling speed, lowering reaction difficulty, and increasing the window of time available for the monkey sprite to intercept the fruit.

---

## Peer-graded Assignment: Document Understanding with a Video Explanation (Variables)

### Snap! Dynamic Regular Polygons Demonstration
- **Project:** Dynamic Polygons: Triangle, Square, and Pentagon (WP_Variables)
- **Tool:** Snap! (UC Berkeley)
- **Video Walkthrough:** https://www.loom.com/share/4ceb74c294884120b00aa3b3b7278db4

#### Program & Concept Description
This video demonstration explains how variables store and update geometric state to dynamically generate multi-sided regular polygons:
- **The purpose of my program is** to draw a sequence of regular polygons across the stage—specifically an orange triangle, a green square, and a blue pentagon—by using variables and loops to dynamically calculate each shape's geometry instead of hardcoding values.
- **My code works by using variables in this part to** store the shape dimensions and update them as the program runs. The variable `num_sides` is initialized to 3 and `side_length` is set to 80. Inside the polygon loop, the sprite repeats `num_sides` times, moves `side_length` steps, and turns counterclockwise by `360 / num_sides` degrees. Between shapes, the script lifts the pen, shifts forward by `side_length + 30` or `50`, and uses `change [num_sides] by 1` so the exact same loop blocks automatically draw the next polygon in the sequence.
- **...and it also uses events in this part to** trigger the program execution via the `when [green flag] clicked` hat block, which initializes the stage, resets the sprite's position, and starts the drawing pipeline from the beginning.
- **The way variables in programming are different than in algebra is** that an algebraic variable represents an unknown or fixed value in a balanced equation (where expressions like $x = x + 1$ are mathematically invalid), whereas a programming variable is a named storage container in memory whose value can be repeatedly updated over time, as demonstrated by the `change [num_sides] by 1` block incrementing the stored value from 3 to 4, and then to 5.

---

## Peer-graded Assignment: Document Understanding with a Video Explanation (Conditional Loops)

### Snap! Conditional Loops Soccer Ball Evasion Demonstration
- **Project:** Conditional Loops: Random Evasion (WP_ConditionalLoops)
- **Tool:** Snap! (UC Berkeley)
- **Video Walkthrough:** https://www.loom.com/share/af88603c10874a1993b206c70d6dc83d

#### Program & Concept Description
This video demonstration explains how indefinite iteration structures real-time responsive behaviors when execution counts cannot be predetermined:
- **The purpose of my program is** to create an interactive dodging game where a soccer ball sprite repeatedly glides to randomized coordinates on the stage until the player successfully intercepts it with their mouse pointer.
- **My code works by using a conditional loop in this part to** continually drive the soccer ball's evasive motion using a `repeat until <touching (mouse-pointer v) ?>` control structure. On every cycle through the loop, the program generates two pseudorandom values—`random number x` between -240 and 240, and `random number y` between -180 and 180—and moves the sprite to that position via `glide (0.1) secs to x: (random number x) y: (random number y)`. At the end of each movement cycle, the predicate condition is re-evaluated, continuing the movement sequence until contact is detected.
- **Conditional loops are different than regular repeats. In my program I can't use a repeat and have to use a conditional repeat because** the exact number of iterations needed to intercept the sprite depends entirely on user reaction speed, mouse tracking accuracy, and randomized coordinate selection. A standard `repeat` block requires a fixed, finite iteration count specified ahead of runtime. Because user interaction creates a non-deterministic stopping point, the program must evaluate the sensing condition dynamically at the boundary of each iteration and terminate only when that specific runtime state is reached.

---

## Peer-graded Assignment: Document Understanding with a Video Explanation (If-Else)

### Snap! If-Else Target Ring Demonstration
- **Project:** Conditional Execution: Target Scoring (WP_If_Else)
- **Tool:** Snap! (UC Berkeley)
- **Video Walkthrough:** https://www.loom.com/share/a73c9d7b16824e7b9d529ff833b88df1

#### Program & Concept Description
This video demonstration highlights how conditional branching and Boolean logic evaluate runtime game state and handle color-based collision scoring:
- **The purpose of my program is** to create an interactive target game where a ball sprite glides to random positions across concentric colored rings for 30 seconds, updating the score based on the color touched when clicked, and providing personalized outcome feedback once time expires.
- **My code works by using if and if-else statements in this part to** evaluate user interactions and overall game outcomes:
  - **Click Collision Evaluation:** Attached to the ball sprite, `when I am clicked` runs three sequential `if` checks using the `touching [color] ?` reporter. If the ball touches red, it changes `score` by `-25` and says `"-25"` for 2 seconds. If touching yellow, it changes `score` by `+25` and says `"+25"`. If touching green, it changes `score` by `+50` and says `"+50"`.
  - **Game-End Outcome Branching:** After the `repeat (10)` glide loop finishes in the green flag script, an `if-else` block checks `<(score) < 0>`. If true, the sprite executes the if-branch and says `"Better luck next time!"` for 2 seconds; if false, it executes the else-branch and says `"Good game!"` for 2 seconds. A subsequent `if` block checks `<(score) > 500>`, saying `"Wow! That's a lot of points!"` for 2 seconds only when that high-score condition is satisfied.
- **If I were to change these if-else conditions like this** by placing the score evaluation blocks inside the `repeat (10)` loop instead of after it, **the program would run differently** by repeatedly triggering the end-game feedback speech bubbles after every single 3-second glide rather than waiting for all 30 seconds of gameplay to conclude.
