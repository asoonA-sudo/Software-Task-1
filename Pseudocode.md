START

DISPLAY "Home Page"

REPEAT
    DISPLAY "1. Flashcards"
    DISPLAY "2. Quiz"
    DISPLAY "3. Exit"

Get user Choice

 IF userChoice = 1 THEN
        CALL FlashcardModule
    ELSE IF userChoice = 2 THEN
        CALL QuizModule
    ELSE IF userChoice = 3 THEN
        DISPLAY "Goodbye"
        STOP PROGRAM
    ELSE
        DISPLAY "Invalid input"
    END IF

PROCEDURE FlashcardModule

SET index = 0

WHILE index < numberOfFlashcards DO

DISPLAY flashcard question

WAIT for user action (click)
    
DISPLAY flashcard answer
   
DISPLAY "Next"
    
index = index + 1

END WHILE

RETURN to main menu

END PROCEDURE



PROCEDURE QuizModule

SET score = 0
SET questionNumber = 0

WHILE questionNumber < totalQuestions DO

DISPLAY question

GET userAnswer

IF userAnswer = correctAnswer THEN
        DISPLAY "Correct"
        score = score + 1
    ELSE
        DISPLAY "Incorrect"
    END IF
    
 questionNumber = questionNumber + 1

END WHILE

DISPLAY "Your score is: " + score

RETURN to main menu

END PROCEDURE

















