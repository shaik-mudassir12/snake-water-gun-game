# snake-water-gun-game
This is a simple snake-water-gun game implemented using if-else statements in python

set={"snake","water","gun"}

print("======welcome to snake water gun game======")
print("Enter your choice: ")
choice=str(input())

def game():
    if(choice=="snake"or"water"or"gun"):
        comp_choice=set.pop()
        if(comp_choice=="snake" and choice=="water"):
            print("computer choice: ",comp_choice)
            print("computer won")
        elif(comp_choice=="water"and choice=="gun"):
            print("computer choice: ",comp_choice)
            print("computer won")
        elif(comp_choice=="gun" and choice=="snake"):
            print("computer choice: ",comp_choice)
            print("computer won")
        elif(comp_choice=="water" and choice=="snake"):
            print("computer choice: ",comp_choice)
            print("You won")
        elif(comp_choice=="snake" and choice=="gun"):
            print("computer choice: ",comp_choice)
            print("You won")
        elif(comp_choice=="gun" and choice=="water"):
            print("computer choice: ",comp_choice)
            print("computer won")

        else:
            print("computer choice:",comp_choice)
            print("Match draw")
    else:
        print("Choose the valid choice")

game()
        

