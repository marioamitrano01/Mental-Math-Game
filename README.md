# Mental Math Dice Game

This Python script implements a **simple dice-based betting game** with basic math operations. Here’s an overview:

1. **Initial Balance**  
   - The game first asks you to enter a starting amount of money (in USD).

2. **Betting and Operation Choice**  
   - Before each round, you place a bet.  
   - You then choose one of four operations: **sum**, **difference**, **multiplication**, or **division**.

3. **Rolling Dice**  
   - The game rolls a different number of dice depending on the chosen operation:
     - **Sum/Difference**: 12 dice  
     - **Multiplication**: 5 dice  
     - **Division**: 3 dice

4. **Answering the Math Problem**  
   - You see the rolled dice values and have **12 seconds** to type in your calculated result.  
   - If your answer is correct (within a small error margin), you **double** your bet.  
   - If you answer incorrectly or run out of time, you lose the bet.

5. **Game History & Plot**  
   - Each round is logged with details about the dice, your guess, and the outcome.  
   - When the game ends (either you run out of money or choose to stop):
     - A summary of all rounds is displayed.
     - If `matplotlib` and `seaborn` are installed, a line plot of your balance over time appears.

## How to Run

1. **Install Dependencies (Optional)**  
   - For colored console output:  
     ```bash
     pip install colorama
     ```
   - For generating the balance plot:  
     ```bash
     pip install matplotlib seaborn
     ```
2. **Launch the Game**  
   ```bash
   python your_script_name.py
   ```
3. **Follow the Prompts**  
   - Input your starting balance.  
   - Place a bet.  
   - Choose an operation (sum, difference, multiplication, or division).  
   - Enter your answer within 12 seconds.

## Key Components

- **`MultipleDice`**: Rolls six-sided dice.  
- **`compute_operation`**: Performs the chosen operation on the dice.  
- **`Player`**: Manages your balance.  
- **`GameUI`**: Handles all user inputs and outputs.  
- **`MarioGame`**: Main class that runs the game flow, including bets, dice rolls, and checking answers.

Enjoy playing, and feel free to customize or extend the code!
