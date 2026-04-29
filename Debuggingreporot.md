# Debugging Report

## Overview

This report explains the problems found while developing the Flashcards + Quiz website and how they were fixed.  
Debugging was important to make sure the website works correctly and gives users a smooth experience.


## Issue 1: Broken Navigation Links

**Problem:**  
Some links did not open the correct pages or showed an error.

**Cause:**  
Incorrect file names or wrong link paths in the HTML.

**Solution:**  
- Checked all links  
- Fixed file names and paths  
- Tested each link

**Result:**  
All navigation links now work correctly.

## Issue 2: Flashcards Not Changing

**Problem:**  
Clicking “Next” did not show a new flashcard.

**Cause:**  
The index value was not updating properly.

**Solution:**  
- Added logic to increase the index value  
- Checked that the index stays within the correct range

**Result:**  
Flashcards now move correctly when the user clicks next.

---

## Issue 3: Quiz Answer Not Working

**Problem:**  
The quiz did not correctly show if an answer was right or wrong.

**Cause:**  
User input was not being compared correctly to the correct answer.

**Solution:**  
- Fixed the comparison logic  
- Made sure answers matched exactly

**Result:**  
Quiz now correctly shows feedback for answers.

---

## Issue 4: Score Not Updating

**Problem:**  
The score did not increase after correct answers.

**Cause:**  
Score variable was not being updated inside the condition.

**Solution:**  
- Added 'score = score + 1` inside correct answer check

**Result:**  
Score now updates properly.

---

## Issue 5: Layout Problems on Mobile

**Problem:**  
Website looked messy on smaller screens.

**Cause:**  
No responsive design rules were applied.

**Solution:**  
- Adjusted layout using simple CSS (e.g. flexible widths)

**Result:**  
Website now displays better on mobile devices.

---

## Testing Methods

- Clicked every button and link
- Tested quiz with correct and incorrect answers
- Checked flashcards multiple times
- Opened website on different screen sizes

---

## Summary

All major issues were identified and fixed.  
The website now works correctly, with proper navigation, working flashcards, and a functional quiz system.  
Debugging improved the reliability and user experience of the website.
