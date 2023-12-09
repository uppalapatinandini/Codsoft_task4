import random

def get_user_choice():
    user_choice = input("Choose rock, paper, or scissors: ").lower()
    while user_choice not in ["rock", "paper", "scissors"]:
        print("Invalid choice. Please choose rock, paper, or scissors.")
        user_choice = input("Choose rock, paper, or scissors: ").lower()
    return user_choice

def get_computer_choice():
    return random.choice(["rock", "paper", "scissors"])

def determine_winner(user_choice, computer_choice):
    if user_choice == computer_choice:
        return "It's a tie!"
    if (
        (user_choice == "rock" and computer_choice == "scissors") or
        (user_choice == "scissors" and computer_choice == "paper") or
        (user_choice == "paper" and computer_choice == "rock")
    ):
        return "You win!"
    return "Computer wins!"

user_score = 0
computer_score = 0

while True:
    user_choice = get_user_choice()
    computer_choice = get_computer_choice()
    print(f"You chose {user_choice}. Computer chose {computer_choice}.")
    
    result = determine_winner(user_choice, computer_choice)
    print(result)
    
    if result == "You win!":
        user_score += 1
    elif result == "Computer wins!":
        computer_score += 1
    
    print(f"User Score: {user_score}, Computer Score: {computer_score}")
    
    play_again = input("Do you want to play again? (yes/no): ").lower()
    if play_again != "yes":
        break

print("Thanks for playing!")
