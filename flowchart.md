   START
     |
     v
Display Home Page
     |
     v
Show Menu Options
     |
     v
Get User Choice
     |
     v     
 -------------------------
| 1 Flashcards | 2 Quiz | 3 Exit |
 -------------------------
  |          |          |
  v          v          v
  
Flashcards  Quiz     END
 Module     Module   Program


   START FLASHCARDS
          |
          v
   Set index = 0
          |
          v
  Is index < total cards?
        /     \
      YES      NO
       |        |
       v        v
Show Question  Return to Menu
       |
       v
Wait for Click
       |
       v
Show Answer
       |
       v
index = index + 1
       |
       v
      LOOP


  START QUIZ
        |
        v
   score = 0
   
   question = 0
        |
        v
Is question < total?
      /    \
    YES     NO
     |       |
     v       v
Show Question  Show Score
     |
     v
Get Answer
     |
     v
Is Answer Correct?
      /    \
    YES     NO
     |       |
     v       v
Add score   Show Incorrect
     |
     v
question + 1
     |
     v
     LOOP
