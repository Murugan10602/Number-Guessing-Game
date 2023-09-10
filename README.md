# Number-Guessing-Game
# Example code: Number Guessing Game
import random

# Generate a random number between 1 and 100
secret_number = random.randint(1, 100)
attempts = 0

while True:
    guess = int(input("Guess the number (1-100): "))
    attempts += 1

    if guess < secret_number:
        print("Try a higher number.")
    elif guess > secret_number:
        print("Try a lower number.")
    else:
        print(f"Congratulations! You guessed the number in {attempts} attempts.")
        break
