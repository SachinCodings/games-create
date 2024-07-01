#[game rock paper task2.txt](https://github.com/user-attachments/files/16051191/game.rock.paper.task2.txt)
random
import random
def game():
    choices = ["rock", "paper", "scissor"]
    computer = random.choice(choices)

    user = input("Enter your choice (rock/paper/scissor): ").lower()
    while user not in choices:
        user = input("Invalid input. Enter your choice (rock/paper/scissor): ").lower()

    print("Computer's choice: ", computer)

    if user == computer:
        print("It's a tie!")
    elif (user == "rock" and computer == "scissor") or (user == "scissor" and computer == "paper") or (user == "paper" and computer == "rock"):
        print("You win!")
    else:
        print("You lose!")

game()
