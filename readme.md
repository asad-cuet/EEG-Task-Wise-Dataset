# EEG-Task-Wise-Dataset

## Description
Here data collected from 50 subjects. Three task was given each subject
Tasks:
   1. Relaxation by closing eyes -> workload_score=0
   2. Medium math -> workload_score=0.5                
   3. Hard math compared to task-2 -> workload_score=1

## Row & Columns
- Each row for 1 second duration. All EEG data in a 1 second duration stored in neuro_raw_eeg in a row.
- neuro_raw_eeg is in array json format, which can be decoded by any programming language.
- There are almost 50 lakhs EEG data points, but as we stored in array of each duration, dataset dimension reduced to 8250x23.
- All columns recorded from Nurosky directly except neuro_relative_<something> columns, its calculated by us.
- is_correct column indicate that is the subject answered correcly of the given math. If correct, all the eeg data during that task assigned as is_correct=1, otherwise is_correct=0