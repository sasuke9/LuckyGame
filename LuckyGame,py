from tkinter import *
from random import sample

window = Tk()
img = PhotoImage(file= "luck_game_photo.png")
imgLbl = Label(window, image= img)
labl1  = Label(window, relief='groove', width= 2)
labl2  = Label(window, relief='groove', width= 2)
labl3  = Label(window, relief='groove', width= 2)
labl4  = Label(window, relief='groove', width= 2)
labl5  = Label(window, relief='groove', width= 2)
labl6  = Label(window, relief='groove', width= 2)

getBtn = Button(window)
resBtn = Button(window)

imgLbl.grid()
labl1.grid()
labl2.grid()
labl3.grid()
labl4.grid()
labl5.grid()
labl6.grid()

getBtn.grid()
resBtn.grid()

imgLbl.grid(row = 1, column = 1, padx = 10)
labl1.grid(row = 1, column = 2, padx = 10)
labl2.grid(row = 1, column = 3, padx = 10)
labl3.grid(row = 1, column = 4, padx = 10)
labl4.grid(row = 1, column = 5, padx = 10)
labl5.grid(row = 1, column = 6, padx = 10)
labl6.grid(row = 1, column = 7, padx = 10)

getBtn.grid(row = 2, column = 2, columnspan = 2)
resBtn.grid(row = 2, column = 6, columnspan = 2)

window.title("Lucky Game || By @941k")
window.resizable(0,0)

labl1.configure(text = "...")
labl2.configure(text = "...")
labl3.configure(text = "...")
labl4.configure(text = "...")
labl5.configure(text = "...")
labl6.configure(text = "...")

getBtn.configure(text = "Get My lucky Number")
resBtn.configure(text = "Reset")

def nums() :
    num = sample(range(1, 50), 6)

    labl1.configure(text=num[0])
    labl2.configure(text=num[1])
    labl3.configure(text=num[2])
    labl4.configure(text=num[3])
    labl5.configure(text=num[4])
    labl6.configure(text=num[5])

    getBtn.configure(state = DISABLED)
    resBtn.configure(state = NORMAL)

def reset ():
    labl1.configure(text="...")
    labl2.configure(text="...")
    labl3.configure(text="...")
    labl4.configure(text="...")
    labl5.configure(text="...")
    labl6.configure(text="...")

    getBtn.configure(state = NORMAL)
    resBtn.configure(state = DISABLED)

getBtn.configure(command = nums)
resBtn.configure(command = reset)

window.mainloop()
