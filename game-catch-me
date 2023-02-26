# CATCH ME IF YOU CAN!

# Estimated time
# 20-30 minutes
#
# Level of difficulty
# Easy
#
# Objectives
# Learn practical skills related to:
#
# using screen coordinates,
# managing widgets with the place manager,
# binding events using the bind() method.

# Scenario

# Write a simple game - an infinite game which humans cannot win.
# Here are the rules:
#
#   the game goes on between TkInter and the user (probably you)

#   TkInter opens a 500x500 pixel window and places a button saying
#   "Catch me!" in the top-left corner of the window;

#   if the user moves the mouse cursor over the button, the button
#   immediately jumps to another location inside the window;
#   you have to assure that the new location is distant enough
#   to prevent the user from making an instant click,

# the button must not cross the window's boundaries during the jump!
# Here is a sample picture for your reference:
#
# Use the place() method to move the button, and the bind()
# method to assign your own callback.

import tkinter as tk

import random


def mouse_over(event):
    a = random.randint(10, 410)
    b = random.randint(10, 480)
    button.place(x=a, y=b)


window = tk.Tk()
window.title("Catch me!")

window.resizable(width=False, height=False)
window.geometry('500x500')

button = tk.Button(window, text="Catch me!")
button.place(x=10, y=10)
button.config(fg="blue", bg="orange")
button.bind("<Enter>", mouse_over)

window.mainloop()
