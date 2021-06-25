# The-Josephus-Problem
import math

soliderNumber = input("How many Soldiers are there: ");

# Declaring variables here
a=0;
r= 1;
l=0;

# Finding power I need to raise 2 to, in order to get soldier number 
# Create while loop to keep raising 2 to a number

while soliderNumber>pow(2,a):
    a+=1

# Until I reach above the soldierNumber, then subtract exponent by 1

if(pow(2,a)>soliderNumber): 
     a = a-1;


# l is equal to the remainder I get

l = soliderNumber - (2**a);


# Position to be in order to survive

pos = 2*l + 1;

# Getting user inputs

answer = input("What position would you like to be in: ")

if answer == pos:
    print("Awesome, you survived!")
else: 
    print("Oh shoot, you died! The correct position was  " +  str(pos))
   



