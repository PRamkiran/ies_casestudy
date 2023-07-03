import random

def roll_dice():
    min_value = 1
    max_value = 6
    
    roll_again = True
    
    while roll_again:
        # Generate a random number between 1 and 6
        dice_value = random.randint(min_value, max_value)
        print("You rolled:", dice_value)
        
        roll_again = input("Do you want to roll again? (yes/no): ").lower() in ["yes", "y"]

roll_dice()
