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

#Write your code below this line 👇
import random
User_choice=int(input("Enter you User Choice: 0,1 or 2\n"))
if User_choice==0:
  print(rock)
elif User_choice==1:
  print(paper)
elif User_choice==2:
  print(scissors)
else:
  print("Invalid input")
Computer_choice=random.randint(0,2)
if Computer_choice==0:
  print(rock)
elif Computer_choice==1:
  print(paper)
else:
  print(scissors)
if User_choice==Computer_choice:
  print("Its a Draw")
elif(User_choice==0 and Computer_choice==2):
  print("You Win")
elif(User_choice==2 and Computer_choice==0):
  print("Computer Wins")
elif(User_choice==1 and Computer_choice==2)or(User_choice==0 and Computer_choice==1):
  print("Computer Wins")
elif(User_choice==2 and Computer_choice==1)or(User_choice==1 and Computer_choice==0):
  print("You Win")
elif(User_choice>2):
  print("Invalid input, Computer Wins")
