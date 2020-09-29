# GUI-continue
This program is in continuation with the GUI program with the addition of using frames here.
Code:

from tkinter import *
root = Tk()


def hello():
    print("You did it\n")

def name():
    print("Hello Mr. Shubham\n")

def age():
    print("Abhi to aap jawaan h sir!\n")



root.title("My gui with harry continue")

root.geometry("255x240")

#Buttons
f1 = Frame(root, bg="brown", borderwidth=6, relief=SUNKEN)
f1.pack(side=LEFT,anchor="nw")

b1 = Button(f1, fg="blue", text="Click me", command=hello)
b1.pack(side=LEFT)

b2 = Button(f1, fg="blue", text="My name", command=name)
b2.pack(padx=4, side=LEFT, fill="y")

b3 = Button(f1, fg="blue", text="Age", command=age)
b3.pack(padx=4, side=LEFT, fill="y")



root.mainloop()
