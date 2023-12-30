# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import the sys module.

### Step 2:
Define a function get_word_count(file_path) to calculate the word count in the file.

### Step 3:
Check if the script is being run as the main program

### Step 4:
Check if the correct number of command-line arguments (i.e., 2) is provided.

### Step 5:
Get the file path from the command-line argument

### Step 6:
Print the word count if it is not None.

### Step 7:
End the program
## PROGRAM:
```python
Program for getting the word count using command line arguments.
Developed by:ARAVIND KUMAR SS 
Register number: 23004721
import sys
def get_word_count(file_path):
    try:
        with open(file_path, 'r') as file:
            content = file.read()
            word_count = len(content.split())
            return word_count
    except FileNotFoundError:
        print(f"Error: File '{file_path}' not found.")
        return None
if name == "main":
    if len(sys.argv) != 2:
        print("Usage: python word_count.py <file_path>")
        sys.exit(1)
    file_path = sys.argv[1]
    word_count = get_word_count(file_path)
    if word_count is not None:
        print(f"Word count in '{file_path}': {word_count}")
```

### OUTPUT:
![python](https://github.com/aravindkumar23004721/command-line-arguments-to-count-word/assets/148962674/f0d8e312-b304-4a81-9758-e98ca53ba952)
![python 1](https://github.com/aravindkumar23004721/command-line-arguments-to-count-word/assets/148962674/a060fedf-2843-4cf7-a0ad-346f12b6084e)
![python 2](https://github.com/aravindkumar23004721/command-line-arguments-to-count-word/assets/148962674/aec20510-597e-49c0-bd5b-b4d9f47e4112)
![python 3](https://github.com/aravindkumar23004721/command-line-arguments-to-count-word/assets/148962674/fe49c865-8e73-432c-9676-46596d41ba9d)
## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
