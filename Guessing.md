```mermaid
flowchart TD
    A([Start Game]) --> B[Generate random number 1 to 100]
    B --> C[/Ask player for a guess/]
    C --> J{Is input a number?}
    J -- No --> K[Display invalid input message]
    K --> C
    J -- Yes --> D{Is the guess correct?}
    D -- Yes --> L[/Tell player their guess is correct/]
    L --> E([Player wins!])
    D -- No --> F{Is the guess too high or too low?}
    F -- Too High --> G[/Tell player it's too high/]
    F -- Too Low --> H[/Tell player it's too low/]
    G --> C
    H --> C
    E --> I([End Game])
```
