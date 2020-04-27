import time
score=0
print("Welcome to the Python Basics quiz")
time.sleep(0.5)
Name= (input("Please enter your name to start the quiz: " ))
print("Hello " +Name.upper()+ " let's get started")
time.sleep(0.5)

def scorePlus():
    global score
    score+=1
    print("You'r score is  ",score)

def scoreMinus():
    global score
    score-=1
    print("You'r score is  ",score)

def q1():
    global score
    print("\nWhat is a correct syntax to output \"Hello World\" in Python?")
    time.sleep(1)
    print(r"A) Print('Hello world')")
    print(r"B) print hello world")
    print(r"C) print 'Hello world'")

    answer= str(input("\nWhat's your answer: "))
    if answer == "a" or answer == "A":
        print("Well done that's the correct answer")
        scorePlus()
    else:
        print("That's the wrong one!!")
        scoreMinus()
    time.sleep(1)
    q2()

def q2():
    global score
    print("\nHow do you insert COMMENTS in Python code?")
    time.sleep(1)
    print("A) #comments")
    print("B) //comments")
    print("C) /*comments*/\n")
    answer = str(input("What's your answer: "))
    if answer == "a" or answer== "A" :
        print("Well done that's the correct answer")
        scorePlus()
    else:
        print("That's the wrong one!!")
        scoreMinus()
    time.sleep(1)
    q3()

def q3():
    global score
    print("\nWhich one is NOT a legal variable name?")
    time.sleep(1)
    print("A) _varname")
    print("B) varName")
    print("C) var-name\n")

    answer = str(input("What's your answer: "))
    if answer == "c" or answer=="C":
        print("Well done that's the correct answer")
        scorePlus()
    else:
        print("That's the wrong one!!")
        scoreMinus()
    time.sleep(1)
    q4()

def q4():
    global score
    print("\nHow do you create a variable with the numeric value 5")
    time.sleep(1)
    print("A) x= int(5)")
    print("B) x= 5")
    print("C) Both are correct\n")

    answer = str(input("What's your answer: "))
    if answer == "c" or answer=="C":
        print("Well done that's the correct answer")
        scorePlus()
    else:
        print("That's the wrong one!!")
        scoreMinus()
    time.sleep(1)
    q5()

def q5():
    global score
    print("\nWhat is the correct file extension for Python files?")
    time.sleep(1)
    print("A) .python")
    print("B) .py")
    print("C) .pyc'\n")

    answer = str(input("What's your answer: "))
    if answer == "b" or answer=="B":
        print("Well done that's the correct answer")
        scorePlus()
    else:
        print("That's the wrong one!!")
        scoreMinus()
    time.sleep(2)
q1()
if(score==5):
    print("\nCongrats you know the basics now")
elif(score>=3):
    print("\nWell done you tried your best, be prepared for the next time")
else:
    print("\nYou should read more")
