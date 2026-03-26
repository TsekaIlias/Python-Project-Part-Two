JOB SHOP SCHEDULING SOLVER & VISUALIZER
=


Description
-----------
This project models, solves, and visualizes Job Shop Scheduling problems. It 
parses text-based problem configurations, applies a scheduling algorithm to 
determine start and end times for machine operations, and provides a graphical 
interface to generate and save Gantt charts. A supplementary script is also 
included for basic UI testing.

Files Included
--------------
1. erotima1.py
   Defines the foundational data structures, including the Operation, Job, and 
   Factory classes. It includes functionality to parse a problem from a text 
   file and sort jobs by their total net execution time.

2. erotima2.py
   Contains the Solution class, which handles the scheduling logic. It uses an 
   eet() method to assign jobs to machines based on the earliest end time and 
   shortest duration, calculating the final makespan.

3. erotima3.py
   A Tkinter-based Graphical User Interface (GUI) named JobShopVisualization. 
   It takes a file path as input, solves the problem using the logic from 
   erotima2.py, and plots a Gantt chart using Matplotlib. It also includes 
   functionality to save the resulting chart as a .png file.

4. buttoncolor.py
   A simple, standalone Tkinter utility that changes the window's background 
   color using "R", "G", and "B" buttons.

Requirements
------------
- Python 3.x
- matplotlib: Required for plotting the Gantt charts. Install via 
  `pip install matplotlib`.
- tkinter: The standard Python GUI library used for the application windows 
  (usually included with Python by default).

How to Run
----------
Open your terminal or command prompt and navigate to the project directory.

To test the core logic and file parsing:
    python erotima1.py <filename.txt>

To run the solver algorithm directly:
    python erotima2.py <filename.txt>

To launch the visualization GUI:
    python erotima3.py
    (Once the window opens, enter the path to your .txt problem file and 
    click "ΕΠΙΛΥΣΗ" to generate the chart).

To test the color picker UI:
    python buttoncolor.py
