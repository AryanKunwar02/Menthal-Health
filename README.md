# Menthal-Health
Mental health is the absence of mental illness or a state of psychological well-being. It's the psychological condition of someone who is emotionally and behaviorally adjusted to a suitable degree.  Subjective well-being, perceived self-efficacy, autonomy, competence, intergenerational reliance, and self-actualization of one's intellectual and emotional potential are just a few of the topics covered.  Mobile applications offer a lot of potentials when it comes to providing high-efficacy mental health therapies. Apps have developed as a feasible tool to bridge the mental health treatment gap, given the global scarcity of psychiatrists and the lack of mental health care access in rural areas. Technology has the potential to revolutionize how mental health care is given and accessed, but it will need the combined mobilization of research, legislation, and design to achieve this goal.


#Team- Mind Map Cache 
#Members: Aryan Kunwar, Aryaman Kunwar, Abibhavan Kumar & Vedaant Kapoor
#Theme:Mental Health



def gettime():
    import datetime
    return datetime.datetime.now()


def log():
    print("Choose your client")
    client = int(input("1. Harry \n2. Rohan \n3. Hammad\n"))
    con = 1
    if client == 1:
        while con == 1:
            print("What do you want to log for Harry?\n")
            choice = int(input("1. Diet \n2. Activity\n"))
            if choice == 1:
                f = open("harry diet.txt", "a")
                data = input("Enter what has Harry Eaten?\n")
                f.write(str([str(gettime())]) + "  " + data + "\n")
                f.close()

            else:
                f = open("harry exercise.txt", "a")
                data = input("How much time has Harry worked out?\n")
                f.write(str([str(gettime())]) + "  " + data + "\n")
                f.close()
            con = int(input("Do you want to log more for Harry? \n1. Yes \n2. No\n"))

    elif client == 2:
        while con == 1:
            print("What do you want to log for Rohan?\n")
            choice = int(input("1. Diet \n2. Activity\n"))
            if choice == 1:
                f = open("rohan diet.txt", "a")
                data = input("Enter what has Rohan Eaten?\n")
                f.write(str([str(gettime())]) + "  " + data + "\n")
                f.close()

            else:
                f = open("rohan exercise.txt", "a")
                data = input("How much time has Rohan worked out?\n")
                f.write(str([str(gettime())]) + "  " + data + "\n")
                f.close()
            con = int(input("Do you want to log more for Rohan? \n1. Yes \n2. No\n"))

    elif client == 3:
        while con == 1:
            print("What do you want to log for Hammad?\n")
            choice = int(input("1. Diet \n2. Activity\n"))
            if choice == 1:
                f = open("hammad diet.txt", "a")
                data = input("Enter what has Hammad Eaten?\n")
                f.write(str([str(gettime())]) + "  " + data + "\n")
                f.close()

            else:
                f = open("hammad exercise.txt", "a")
                data = input("How much time has Hammad worked out?\n")
                f.write(str([str(gettime())]) + "  " + data + "\n")
                f.close()
            con = int(input("Do you want to log more for Hammad? \n1. Yes \n2. No\n"))


def retrieve():
    con = 1
    while con == 1:
        print("Choose your client")
        client = int(input("1. Harry \n2. Rohan \n3. Hammad\n"))
        if client == 1:
            print("What do you want to retrieve for Harry?\n")
            choice = int(input("1. Diet \n2. Activity\n"))
            if choice == 1:
                f = open("harry diet.txt", "r")
                print(f.readlines())
                f.close()

            else:
                f = open("harry exercise.txt", "r")
                print(f.readlines())
                f.close()

        elif client == 2:
            print("What do you want to retrieve for Rohan?\n")
            choice = int(input("1. Diet \n2. Activity\n"))
            if choice == 1:
                f = open("rohan diet.txt", "r")
                print(f.readlines())
                f.close()

            else:
                f = open("rohan exercise.txt", "r")
                print(f.readlines())
                f.close()

        elif client == 3:
            print("What do you want to retrieve for Hammad?\n")
            choice = int(input("1. Diet \n2. Activity\n"))
            if choice == 1:
                f = open("hammad diet.txt", "r")
                print(f.readlines())
                f.close()

            else:
                f = open("hammad exercise.txt", "r")
                print(f.readlines())
                f.close()
    con = int(input("Do you want to retrieve any more details? \n1. Yes \n2. No\n"))


print("\tWelcome to Health care Management System")
ch = int(input("What do you want to do? \n1. Log \n2. Retrieve\n"))
if ch == 1:
    log()
elif ch == 2:
    retrieve()
else:
    print("Wrong Input. Please try again.\n")
