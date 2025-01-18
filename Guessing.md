```mermaid
flowchart TD
    Start([Start]) --> A[Computer generates number between a certain range]
    A --> B[Computer tells user to guess a number between # to #]
    B --> C[User enters number within the range]
    C --> D[Computer evaluates that number is too high]
    D --> E[Tells user they're too high and ask if they want to try again]
    E --> F[Try Again]
    F --> B
    E --> J[Don't try again]
    J --> End([End])
    C --> K[Computer evaluates that number is correct]
    K --> L[Congrats you win! Play Again?]
    L --> M[Play Again]
    M --> A
    L --> N[Don't play again]
    N --> End([End])
    C --> O[Computer evaluates that number is too low]
    O --> P[Tells user they're too low and ask if they want to try again]
    P--> Q[Try Again]
    Q --> B
    P --> R[Don't try again]
    R --> End([End])
    B --> S[User enters a non-number]
    S --> T[Tell user that their answer is not a number and to try again]
    T --> B

    B --> U[User enters number not within the range]
    U --> V[Tell user that their answer is not within the specified range and to try again]
    V --> B 
```    
## Describing The Flowchart  

The first step after starting the game is for the computer to generate a random number. From there, the computer asks the user to guess a number, giving a range for them to guess a number. After that, the computer has essentially three decisions based on the user's input. If the user either gives a number outside the range provided **or** gives a non-number answer, the computer will then proceed to tell the user to try again with an answer that is either a number or within the range depending on the choice.   
If the user gives an answer that is both within the range _and_ a is a number, the computer again has three different outcomes. If the answer is lower than the correct number generated, it will tell the user this and ask if they want to try again or end the game. If they do want to try again, it will go back to the screen where the computer asks them to guess a number between the already predetermined range. If the user does not want to try again, the game will end.  
If the answer is higher than the correct number generated, it will tell the user this and ask if they want to try again or end the game. If they do want to try again, it will go back to the screen where the computer asks them to guess a number between the already predetermined range. If the user does not want to try again, the game will end.  
If the answer is correct, it will display a congratulatory message that they win and if they want to play again. If yes, the computer will once again generate a new number between a certain range, and ask them to guess a number, continnuing the flowchart from the beginning. If they do not want to play again, the game will end.