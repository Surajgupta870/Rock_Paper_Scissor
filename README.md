# Rock_Paper_Scissor

rock = '''

        _______
    ---'   ____)
            (_____)
            (_____)
            (____)
    ---.__(___)
    
'''


paper = '''

        _______
    ---'   ____)____
              ______)
              _______)
             _______)
    ---.__________)
    
'''

scissors = '''

            _______
        ---'   ____)____
                  ______)
               __________)
              (____)
        ---.__(___)

    
'''
import random

user_choice=int(input("what do you choose? Type 0 for rock, 1 for paper and 2 for scissors.\n"))

RPS=[rock,paper,scissors]

print(RPS[user_choice])

print ("computer choose:")

computer_choice=random.randint(0,2)

print(RPS[computer_choice])

if user_choice == 0 and computer_choice == 2:
    
    print("You Win!")

elif computer_choice > user_choice:
    
    print("You lose.")

if computer_choice==0 and user_choice==2:
    
    print("You lose.")

elif user_choice > computer_choice:
    
    print("You Win!")

else:
    
    print("Its draw.")

