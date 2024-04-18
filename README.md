# Rock_Paper_Scissors
#Multiple time user can play the game
#input user
#input computer
#Rock beat scissors
#Paper beat rocks
#Scissor beat paper

import random
while True:
    user=int(input("Enter your choice:\n 1->Rock\n 2->Paper \n 3->Scissor"))
    computer= random.randint(1,3)
    print("Computer choice",computer)
    
    if(user==computer):
        print(f"Your choice {user} and computer choice {computer} so, both Tie!")
    elif(user==1):
        if(computer==3):
            print(f"Your choice {user} and computer choice {computer} so, you win!")
        else:
            print(f"Your choice {user} and computer choice {computer} so, Computer win!")
    elif(user==2):
        if(computer==1):
            print(f"Your choice {user} and computer choice {computer} so, you win!")
        else:
            print(f"Your choice {user} and computer choice {computer} so, Computer win!")
    elif(user==3):
        if(computer==2):
            print(f"Your choice {user} and computer choice {computer} so, you win!")
        else:
            print("Computer win!")
    exit = input("\nWould you like to play game? Y/N")
    if exit=="N":
        break  
