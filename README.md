# Menthal-Health
Mental health is the absence of mental illness or a state of psychological well-being. It's the psychological condition of someone who is emotionally and behaviorally adjusted to a suitable degree.  Subjective well-being, perceived self-efficacy, autonomy, competence, intergenerational reliance, and self-actualization of one's intellectual and emotional potential are just a few of the topics covered.  Mobile applications offer a lot of potentials when it comes to providing high-efficacy mental health therapies. Apps have developed as a feasible tool to bridge the mental health treatment gap, given the global scarcity of psychiatrists and the lack of mental health care access in rural areas. Technology has the potential to revolutionize how mental health care is given and accessed, but it will need the combined mobilization of research, legislation, and design to achieve this goal.


#Team- Mind Map Cache 
#Members: Aryan Kunwar, Aryaman Kunwar, Abibhavan Kumar & Vedaant Kapoor
#Theme:Mental Health


def getdate():
    import datetime
    return datetime.datetime.now()

def take(k):
    if k==1:
        c=int(input("Enter 1 for Exercise and 2 for Diet"))
        if c==1:
            value=input("Type Here...\n")
            with open("harryexercise.txt", "a") as f:
                
                f.write(str(getdate()) + ":" + value + "\n")   
                print("Successfully Updated")

        elif c==2:
            value=input("Type Here...\n")
            with open("harrydiet.txt", "a") as f:
                
                f.write(str(getdate()) + ":" + value + "\n")   
                print("Successfully Updated")

    elif k==2:
        c=int(input("Enter 1 for Exercise and 2 for Diet"))
        if c == 1:
            value = input("Type Here...\n")
            with open("rohanexercise.txt", "a") as f:
                
                f.write(str(getdate()) + ":" + value + "\n") 
                print("Successfully Updated")

        elif c == 2:
            value = input("Type Here...\n")
            with open("rohandiet.txt", "a") as f:
                
                f.write(str(getdate()) + ":" + value + "\n")  
                print("Successfully Updated")

    elif k==3:
        c = int(input("Enter 1 for Exercise and 2 for Diet"))
        if c == 1:
            value = input("Type Here...\n")
            with open("hammadexercise.txt", "a") as f:
                
                f.write(str(getdate()) + ":" + value + "\n") 
                print("Successfully Updated")

        elif c == 2:
            value = input("Type Here...\n")
            with open("hammaddiet.txt", "a") as f:
                
                f.write(str(getdate()) + ":" + value + "\n")  
                print("Successfully Updated")
    else:
        print("Please enter valid input: 1-Harry, 2-Rohan, 3-Hammad")

def retrieve(k):
    if k==1:
        c = int(input("Enter 1 for Exercise and 2 for Diet"))
        if c==1:
            with open("harryexercise.txt") as g:
                print(g.read())
        elif c==2:
            with open("harrydiet.txt") as g:
                print(g.read())
    elif k==2:
        c = int(input("Enter 1 for Exercise and 2 for Diet"))
        if c == 1:
            with open("rohanexercise.txt") as g:
                print(g.read())
        elif c == 2:
            with open("rohandiet.txt") as g:
                print(g.read())

    elif k==3:
        c = int(input("Enter 1 for Exercise and 2 for Diet"))
        if c == 1:
            with open("hammadexercise.txt") as g:
                print(g.read())
        elif c == 2:
            with open("hammaddiet.txt") as g:
                print(g.read())
    else:
        print("Please enter valid input: 1-Harry, 2-Rohan, 3-Hammad")

print("Welcome to Health Management System:")
a=int(input("Enter 1 to log the value and 2 for retrieve"))
if a==1:
    b=int(input("Please enter: 1-Harry, 2-Rohan, 3-Hammad"))
    take(b)
else:
    b=int(input("Please enter: 1-Harry, 2-Rohan, 3-Hammad"))
    retrieve(b)
