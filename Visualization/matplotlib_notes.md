# 📘 DATA VISUALIZATION – MATPLOTLIB BASICS (REVISION NOTES)

---

## 🔹 1. Importing Libraries

### python
** import pandas as pd
** import numpy as np
** import matplotlib.pyplot as plt

## 📌 Notes:
pandas (pd) → Data handling (tables, CSV files)
numpy (np) → Numerical operations (arrays, math)
matplotlib.pyplot (plt) → Data visualization (graphs)
## 🧠 Key Point:
plt acts like a drawing canvas
Flow: Data → Process → Visualize
🔹 2. Creating Data using NumPy
x = np.linspace(0,5,11)


## 📌 Definition:
linspace() generates equally spaced values in a given range.

### 📌 Syntax:
np.linspace(start, stop, num_points)

### 📌 Parameters:
start → Starting value
stop → Ending value
num_points → Total values required
🧠 Logic:
Used to create smooth continuous data
Helpful in plotting curves
🔹 3. Broadcasting (NumPy Concept)
y = x**2


## 📌 Definition:
Broadcasting means applying operations element-wise automatically on arrays.

### 🧠 Logic:
Each element of x is squared → stored in y
No need for loops
### 📌 Advantages:
Faster computation
Cleaner code
Important for ML operations
🔹 4. Line Plot using Matplotlib
plt.plot(x,y)


## 📌 Definition:
Creates a line graph between x and y values.

### 📌 Syntax:
plt.plot(x, y, color, linestyle, linewidth, marker)
### 📌 Important Parameters:
x → X-axis data
y → Y-axis data
color → Line color
linestyle → Line pattern (-, --, :)
linewidth → Thickness of line
marker → Points (o, *, .)
### 🧠 Logic:
Plots points (x[i], y[i])
Joins them → forms a curve/line
🔹 5. Adding Title and Labels
plt.title("Sample Data")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
### 📌 Purpose:
Makes graph understandable and meaningful
### 📌 Syntax:
plt.title(label)
plt.xlabel(label)
plt.ylabel(label)
### 🧠 Logic:
Without labels → graph has no context
Used in reports, projects, presentations
🔹 6. Subplots in Matplotlib
plt.subplot(nrows, ncols, index)


### 📌 Definition:
Used to create multiple plots in a single figure

### 📌 Parameters:
nrows → Number of rows
ncols → Number of columns
index → Position of graph (starts from 1)
### 📌 Example:
plt.subplot(1,2,1)
plt.plot(x,y)
plt.subplot(1,2,2)
plt.plot(y,x)

### 🧠 Logic:
Divides screen into grid
Each subplot occupies a position
🔹 7. Matplotlib Working (Important Concept)
### 📌 Structure:
Figure → Entire canvas
Axes → Individual graph
### 🧠 Flow:
Figure → Axes → Plot → Show
🔹 8. Complete Basic Code Example
import numpy as np
import matplotlib.pyplot as plt

## Data creation
x = np.linspace(0,5,11)
y = x**2

## Plotting
plt.plot(x,y)

## Labels
plt.title("Sample Data")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")

## Show graph
plt.show()
🔥 Quick Revision (1-Min Recap)
linspace() → generate data
Broadcasting → element-wise operation
plot() → create graph
title/xlabel/ylabel → add meaning
subplot() → multiple graphs
Matplotlib → Figure + Axes system 
