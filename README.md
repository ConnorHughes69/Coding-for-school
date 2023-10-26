import sys

def GetInput(Message):
    userinput = ""
    nn=0
    while len(userinput)==0:
        userinput=input(Message)
        nn+=1
        if nn>5:
            print("What is wrong with you?")
            print("we are done here")
            sys.exit(1)      
    return userinput

print("Welcome to chat box")
userinput = GetInput("start your conversation")

if userinput.lower()=="hi" or userinput.lower()=="hello":
    print("hello, how are you:")
    userinput = GetInput("You are a moron")
else:
    print("blah")
    print("hello, how are you:")
    userinput = GetInput("I hate you")

if userinput=="bad" or userinput.lower()== "terrible":
    print("I am sorry to hear that")
elif userinput=="good":
    print("I am glad to hear that")
else:
    print("ok")

print("What did you do today")
userinput = GetInput("")
print("That is so awesome")



print("thank you for talking with me and I hope you have a good day")

