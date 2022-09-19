Task 2: Computational thinking


Question 1: What is the most powerful computer? Glad you asked. Watch this video about Sierra Computer. Describe below points that surprised you the most.
Sierras originate has to do with the nuclear testing and the removing of armsn from nations

How ever they didnt disarm their nukes

Government intervention in use of sierra

Sieraa is going to simulat military questions regarding the relainbilty of nuclear warheads

These will predit wheter there will be warheads are viable

In combinations of 12 other supercomputers

People working only care about getting answers

Prioriatizing weapons over reseasch to help people


Question 2: Supercomputers are currently used to investigate solutions to real life problems from cancer research, Ai, economics, or brain simulation. 
Military uses are also one major force behind the development of these machines.

Analyze the benefits and possible drawbacks of developing supercomputers in our modern world? Should we do it?
The more and more developed these supercomputers get the more likey they are to solve certain problems for the betterment of the world 
however the risk for the wrongful use or dangerous use of these powerful machines also increase. Meaning there is a high risk high reward situation.
Which is mainly dependant on the government. Considering how unreliable the government can be this becomes extremely risky. However the benefits that 
could come from these computers is also very vast and could help people throughout their daily lives.

Question 3: Identify the most advanced computer in your Country (What, specs, location, uses). 
There is no official super computer in armenia however there is a prompemt crypto mining presensese in armenia 
so the most powerful computer in armenia is probably a privately owned crypto miner



Programming task

Save your program in a file called task1.md. In a school there are 2400 students and each student uses one locker. Each locker has a unique number from 1 to 2400. The lockers are to be painted in four colors: red, white, yellow and blue, in order of locker numbers, as shown in the following table.link

The pattern of colors continues in this manner. For example, locker number 15 will be painted yellow.

Task 1: Create a program and the flow diagram that shows the colors of all the lockers from 1 to 2400
With in task 4

Task 2: Using the program above, create another program that allows the user to enter a number and the program outputs the color that should be used in the locker.
With in task 4

[HL] Task 3: Create a program that receives a color from the user, validates the input,  and outputs the numbers of the lockers of the color provided. 
Use at least 10 different functions for Manipulating Strings (Learning Log Item 19)
Im not sure how to do it 

[HL] Task 4: Given a list of names of students in the format lastname, firstname, create a program that assigns an email address and a locker to each 
student and savesthe results in a file in the format lastname, firstname, email, locker.
[Evidence for code](TASK 1 out of 2.jpg     )
[](TASK 2 out of 2.jpg)
```.py
import random
x = random.randint(1,2400)

max_num_tries = 5
while not x and max_num_tries > 0:
    max_num_tries = max_num_tries - 1
    x = input(f"Not Perfect, you have {max_num_tries} chances left. Please enter an integer:")

number_lockers = 2400

if int(x) and int(x)%4 == 0:
    colors = ["blue","red", "white", "yellow"]
    color = colors[int(x)%4]


if int(x) and int(x)%4 == 1:
    colors = ["blue","red", "white", "yellow"]
    color = colors[int(x)%4]


if int(x) and int(x)%4 == 2:
    colors = ["blue","red", "white", "yellow"]
    color = colors[int(x)%4]


if int(x) and int(x)%4 == 3:
    colors = ["blue","red", "white", "yellow"]
    color = colors[int(x)%4]

first_name = input("Enter first Name:")
last_name = input("Enter last name:")
graduation_year = int(input("Enter Graduation Year:"))


print (f"Your email is {graduation_year}.{first_name}.{last_name}@uwcisak.jp and Locker No {x} is color {color.upper(). center(50,'.')}")


