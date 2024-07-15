# Duck Duck Go ChatBot with Feedback System

## Overview

This project involves creating a feedback system where users can submit their feedback regarding answers they receive. The feedback includes a rating and a comment or suggestion. The feedback is stored in a CSV file, and statistics about the feedback can be calculated and displayed.


## Files and Directories

- `main.py`: Main script for taking user queries, providing answers, and collecting feedback.
- `functions/take_feedback.py`: Contains the `feedback()` function for collecting feedback.
- `feedback_stats.py`: Script for reading feedback data and calculating statistics.
- `Feedback data/Feedback.csv`: CSV file for storing feedback data. Automatically created if it doesn't exist.

## Usage

### Running the Main Script

1. Navigate to the project directory.
2. Run the `main.py` script:
    ```bash
    python main.py
    ```
3. The script will prompt you for a question.
4. It will perform a search, provide an answer, and then ask for your feedback.

### Collecting Feedback

The `feedback()` function in `functions/take_feedback.py` prompts the user to rate their satisfaction from 1 to 5. If the rating is 3 or lower, the user will be asked to provide additional comments or suggestions.

### Storing Feedback

The feedback is stored in `Feedback.csv` within the `Feedback data` directory. If the directory or file does not exist, they will be created automatically.

### Viewing Feedback Statistics

1. Navigate to the project directory.
2. Run the `feedback_stats.py` script:
    ```bash
    python feedback_stats.py
    ```
3. The script will print the average satisfaction rating and display each rating with the corresponding comment.
