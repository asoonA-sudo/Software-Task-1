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
