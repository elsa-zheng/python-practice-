print("HEELLOOO! welcome to the adventure game!")
print("you wake up in a mysterious cave…")
print("what do you do?")
print("1. go left")
print("2. go right")

choice = input("choose between 1 and 2 : ")
if choice == "1":
    print("oops you died by being eaten by a dragon")
if choice == "2":
    print("okayy level up!!")
    while True:
        print("you now have 2 choices")
        break
    print("1. go upwards")
    print("2. go downwards")
    chosen_number = input("choose another number: ")
    if chosen_number == "1":
        print("YOU DIED")
    if chosen_number == "2":
        print("yay, you're close to the treasure!")
        while True:
            print("nows ur last test…")
            break
        print("what is ur name?")
        name = input("enter your name: ")
        print(f"ok {name} you may leave now;)nothing to see here lallalalalalal")
        
        
print("NOW GUESS THE SECRET NUMBER")
import random
attempts = 0
secret = random.randint(1,20)
while True:
    guess = int(input("enter ur number: "))
    
    attempts += 1
    
    if secret > guess:
        print("TOO SMALL")
    elif secret < guess:
        print("TOO BIG")
    else:
        print(f"YOU GOT IT RIGHT IN {attempts} TRIESSSS")
        break
