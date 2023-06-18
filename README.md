Name: Aman Hogan-Bailey
Date: 03/2023

Programming Language: 3.11.2 64 Python
Environement: VsCode and Microsoft CMD command line prompt

# Structure

The program structure is as follows:

## `algo_main.py`

The driver code is specified in `algo_main.py`. This Python file is responsible for several functions related to sorting algorithms and includes the `AlgorithmData` class that holds information about the data and the execution time of a sorting algorithm. It calls the following Python modules:

## `algo_sorting.py`

This file contains several sorting algorithms implemented in Python:

1. `merge_sort(arr, data)`: Performs merge sort on the array.
2. `heap_sort(arr, data)`: Implements the heap sort algorithm.
3. `heapify(arr, n, i)`: A helper function for the `heap_sort` function.
4. `quick_sort(arr)`: Implements the quick sort algorithm by recursively partitioning the array into two sub-arrays around a pivot until the base case of an array with a single element is reached.
5. `quick_sort_median(arr)`: Partitions the array into three sub-arrays around the pivot and recursively sorts them before concatenating them with the pivot sub-array.
6. `selection_sort(arr, data)`: Finds the minimum element in the unsorted part of the array and swaps it with the first element of the unsorted part.
7. `insertion_sort(arr, data)`: Implements the insertion sort algorithm.
8. `bubble_sort(arr, data)`: Implements the bubble sort algorithm.

## `algorithm_view.py` (GUI)

This module is a GUI application that allows the user to choose and compare sorting algorithms on randomly generated arrays of integers. It includes the following functions:

- `initialize_gui()`: Creates a main window for the GUI, where the user can input the desired size of the array to be sorted and select a sorting algorithm using buttons.
- `array_to_screen()`: Creates a new window to display the details of the selected sorting algorithm, including the algorithm name, array size, start time, end time, run time, bytes per microsecond, and unsorted array. It imports the `tkinter` module and uses its functions and widgets to create the GUI, as well as several functions from the `algo_main` module and `algo_sorting` module to perform the actual sorting.

## `algo_graph.py`

This Python module, named `algo_graph.py`, is responsible for plotting a graph of input sizes versus runtimes in microseconds. It includes the following function:

- `graphing()`: Adds the `graph_name` to the `graph_names` list and prints a message indicating that it is graphing the specified algorithm.

## Additional Files

- `inputs.txt`: This file is included but not necessary since the arrays are randomized using the Python `random` module.
- `<sorting name>.png`: After graphing an algorithm, the program will save a PNG image of the graph in the current running directory.

# Program Logic

The program follows the following logic:

1. The user is prompted to a screen that displays a variety of sorting algorithms (such as Merge Sort, Heap Sort, Quick Sort, etc.) to sort an array of random integers. The program shows the results of each algorithm in real-time.
2. The user must enter the desired array size and press 'Submit'.
3. The user can then interact with the program by choosing an algorithm to run, comparing the results of two algorithms, and graphing the run-time of an algorithm.
4. The GUI displays the details of the algorithm's performance, including the start and end time, run-time, number of bytes per microsecond, unsorted and sorted arrays, in a separate window.

# How to Run

There are two ways to run this program:

## Windows CMD:
1. Unzip the downloaded file.
2. Open your Windows terminal.
3. Make sure you have Python version 3 or higher installed.
4. Navigate to the directory where the source code, specifically 'algo_main.py', is located using the command: `cd C:\Users\ .... \algo_main.py`
5. Run the program by executing the following command in the command-line: `python algo_main.py`
6. The code should then output the results.

## VScode:
1. Unzip the downloaded file.
2. Open the folder in VScode and select 'Trust this folder' if prompted.
3. Set up your VScode to have a Python Environment:
   - Hold down SHIFT+CTRL+P and select 'Python: Select Interpreter'
   - Choose the path where Python is installed on your system.
4. Find the 'algo_main.py' file in the folder and right-click on it.
5. Select 'Run Python File in Terminal'.
   - This will open a terminal in VScode using a Python interpreter.
6. Now, with the terminal open, enter the command `python algo_main.py`.
7. The program should then run and print the necessary outputs.
