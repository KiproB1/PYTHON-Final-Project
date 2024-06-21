# PYTHON-Final-Projectimport time

def intro():
    print("Welcome to the Text Adventure Game!")
    time.sleep(2)
    print("You find yourself in a mysterious house...")
    time.sleep(2)
    print("Your goal is to find the treasure hidden somewhere inside.")
    time.sleep(2)
    print("Let's begin!\n")

def choose_action():
    print("\nWhat do you want to do?")
    print("1. Open the door")
    print("2. Look for a key")
    print("3. Quit")
    choice = input("Enter your choice (1/2/3): ")
    return choice

def room_one():
    print("\nYou are in Room 1.")
    time.sleep(1)
    print("There is a locked door in front of you.")
    choice = choose_action()
    if choice == '1':
        print("The door is locked. You need a key!")
        room_one()
    elif choice == '2':
        print("You found a key!")
        time.sleep(1)
        room_two()
    elif choice == '3':
        print("Game Over. You quit the game.")
        quit()
    else:
        print("Invalid choice. Try again.")
        room_one()

def room_two():
    print("\nYou unlocked the door with the key!")
    time.sleep(1)
    print("You are in Room 2.")
    time.sleep(1)
    print("There is a chest in the middle of the room.")
    choice = choose_action()
    if choice == '1':
        print("You opened the chest and found the treasure!")
        time.sleep(1)
        print("Congratulations! You won the game.")
        quit()
    elif choice == '2':
        print("There's nothing else to find here.")
        room_two()
    elif choice == '3':
        print("Game Over. You quit the game.")
        quit()
    else:
        print("Invalid choice. Try again.")
        room_two()

def main():
    intro()
    room_one()

if __name__ == "__main__":
    main()
Welcome to the Text Adventure Game!
You find yourself in a mysterious house...
Your goal is to find the treasure hidden somewhere inside.
Let's begin!

You are in Room 1.
There is a locked door in front of you.

What do you want to do?
1. Open the door
2. Look for a key
3. Quit
Enter your choice (1/2/3): 2
You found a key!

You unlocked the door with the key!
You are in Room 2.
There is a chest in the

