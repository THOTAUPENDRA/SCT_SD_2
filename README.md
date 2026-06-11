#  Guess the Number Game

A simple and interactive **Number Guessing Game Web App** built using **Python** and **Streamlit**.

The computer randomly selects a number between **1 and 100**, and the player tries to guess it. The app provides hints like **Too High** or **Too Low** until the correct number is found.

##  Features

- Random number generation between 1 and 100
- Interactive input field for guesses
- Tracks number of attempts
- Provides hints:
  -  Too Low
  -  Too High
- Displays success message after correct guess
- Start a new game anytime
- Uses Streamlit session state to maintain game progress

##  Technologies Used

- Python
- Streamlit
- Random Module

##  Project Structure

```
Guess-Number-Game/
│
├── app.py              # Main Streamlit application
├── README.md           # Project documentation
└── requirements.txt    # Required dependencies
```

##  Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Guess-Number-Game.git
```

### 2. Navigate to the project folder

```bash
cd Guess-Number-Game
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

##  Run the Application

Run the Streamlit app using:

```bash
streamlit run app.py
```

The game will open in your browser.

##  How to Play

1. The computer selects a random number from **1 to 100**.
2. Enter your guess.
3. Click **Submit Guess**.
4. Follow the hints:
   -  "Too low! Try again."
   -  "Too high! Try again."
5. Keep guessing until you find the number.
6. Click **New Game** to restart.

##  Game Logic

The application uses:

- `random.randint()`  
  - Generates a random secret number.

- `st.session_state`
  - Stores:
    - Secret number
    - Number of attempts
  - Keeps data even when Streamlit refreshes the page.

##  Example

```
I'm thinking of a number between 1 and 100.

Enter your guess: 50

 Too high! Try again.

Enter your guess: 25

 Too low! Try again.

Enter your guess: 37

 Congratulations!
You guessed the number 37 in 3 attempts.
```

##  Requirements

Create a `requirements.txt` file:

```
streamlit
```

##  License

This project is open-source and available under the MIT License.
