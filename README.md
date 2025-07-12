# Graph-Visualization-Exercise 
Malawi Districts Graph Visualization

Project Objective

This project visualizes the connections between Malawi’s 28 districts using a force-directed graph layout. The goal is to take an initial set of rough (x, y) positions and district connections, then optimize the layout so that:
- Nodes (districts) are evenly spread out
- Connected nodes are placed closer together
- Overlapping and edge crossings are reduced for clarity

---

Problem Overview

We’re working with 28 districts, each represented by a node with an initial normalized position (between 0 and 1). The connections between districts are defined in an adjacency list format.

The initial layout is often messy, with overlapping labels and tangled lines. This project uses a layout algorithm to reposition the nodes in a way that’s easier to read and visually informative.

---

Algorithm Used: Force-Directed Layout (Fruchterman-Reingold)

To clean up the layout, a simplified version of the Fruchterman-Reingold force-directed algorithm was used, which works by simulating physical forces:

- Attraction: Connected nodes are pulled toward each other like they’re linked by springs.
- Repulsion: All nodes push away from each other to avoid overlapping.

This process runs for multiple iterations until the system reaches a balanced state, producing a neater and more readable layout.

---

 How to Run the Project

Option 1: download/Open raw `index.html` file:
    Open the `index.html` file in any modern web browser (e.g., Chrome, Firefox, Edge).
    You can do this by double-clicking the file or by right-clicking and selecting "Open with"> "Your Web Browser".
  
Option 2: Clone the repository:
    ```bash
   git clone https://github.com/PreciousChingani/malawi-districts-graph.git
   
Option 3: Navigate to the project directory:
    ```bash
    cd malawi-districts-graph
    ```
---

 Results

A graph with all 28 Malawi districts shown as labeled nodes (circles).
Connections between districts are represented as lines (edges).
A cleaned-up layout after applying 300 iterations of the layout algorithm.
Final (x, y) coordinates for each district are shown in:
A log box on the web page.
The browser’s developer console (F12 > Console).
*Screenshots are provided in the Repo.

---
Dependencies

No external libraries or frameworks are needed.
This project runs entirely on:
-HTML
-CSS
-Vanilla JavaScript
-SVG (Scalable Vector Graphics)
*Everything is handled by the browser, so no installation or build process is required.
