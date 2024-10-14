# Guessing Game

# Set the secret number
secret_number = 42

# Ask the user to guess the number
print("Guess a number between 1 and 100:")

# Get the user's input
user_guess = int(input())

# Check if the user's guess is correct
if user_guess == secret_number:
    print(" Congratulations! You guessed the correct number.")
else:
    print(" Sorry, your guess is incorrect. The correct answer is", secret_number)

# Bonus: Add a loop to allow the user to play again
while True:
    print("Do you want to play again? (yes/no)")
    response = input()
    if response.lower() == "yes":
        # Reset the user's guess
        user_guess = int(input("Guess a number between 1 and 100:"))
        if user_guess == secret_number:
            print(" Congratulations! You guessed the correct number.")
        else:
            print(" Sorry, your guess is incorrect. The correct answer is", secret_number)
    elif response.lower() == "no":
        print("Thanks for playing!")
        break
    else:
        print("Invalid response. Please enter yes or no.")
