# Number Guessing Game, Flowchart
## Description 
1. **Start**: The game begins by initializing the process.
2. **Randome Number Generation**: The program generates a randome number within a specific range.
3. **User Input**: The user is prompted to guess the number.
4. **Validation**: The program check if the guess is valid. If not it'll ask for another input.
5. **Check Guess**: If the guess is correct, the game ends, and a congratulatory message appears. If the guess is incorrect, feedback is provided, and user is prompted to try again.
6. **End Game**: Once the correct guess is made, the game gives options to exit or try again.
   
''' mermaid
flowchart TD
  Start([Start Game]) --> A[Generate Random Number]
  A --> B[Prompt User for Guess]
  B --> C{Is Guess Valid?}
  C --> |No| B
  C --> |Yes| D{Is Guess Correct?}
  D --> |Yes| E[Display "Congratulations! You Win!"]
  E --> F[Ask User to Play Again or Exit]
  D --> |No, Too High| G[Display "Too High! Try Again"]
  D --> |No, Too Low| H[Display "Too Low! Try Again"]
  G --> B
  H --> B
  F -->|Play Again| A
  F -->|Exit| End([End])
'''
