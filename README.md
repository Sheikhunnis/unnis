# unnis.   Tik tok toe game code 

from tkinter import *
from tkinter import messagebox
root=Tk()
global x,o

def over():
	
	
	global btn1,btn2,btn3
	if btn1["text"]=="o" and btn2["text"]=="o" and btn3["text"]=="o":
		btn1.config(bg="black")
		btn2.config(bg="black")
		btn3.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
		
	elif btn4["text"]=="o" and btn5["text"]=="o" and btn6["text"]=="o":
		btn4.config(bg="black")
		btn5.config(bg="black")
		btn6.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
	elif btn7["text"]=="o" and btn8["text"]=="o" and btn9["text"]=="o":
		btn7.config(bg="black")
		btn8.config(bg="black")
		btn9.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
		
	elif btn1["text"]=="o" and btn4["text"]=="o" and btn7["text"]=="o":
		btn1.config(bg="black")
		btn4.config(bg="black")
		btn7.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
		
	elif  btn2["text"]=="o" and btn5["text"]=="o" and btn8["text"]=="o":
		btn2.config(bg="black")
		btn5.config(bg="black")
		btn8.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
		
	elif  btn3["text"]=="o" and btn6["text"]=="o" and btn9["text"]=="o":
		btn3.config(bg="black")
		btn6.config(bg="black")
		btn9.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
		
	elif  btn1["text"]=="o" and btn5["text"]=="o" and btn9["text"]=="o":
		btn1.config(bg="black")
		btn5.config(bg="black")
		btn9.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
		
	elif  btn3["text"]=="o" and btn5["text"]=="o" and btn7["text"]=="o":
		btn3.config(bg="black")
		btn5.config(bg="black")
		btn7.config(bg="black")
		messagebox.showinfo("","o win!!")
		root.destroy()
	
	elif btn1["text"]=="x" and btn2["text"]=="x" and btn3["text"]=="x":
		btn1.config(bg="black")
		btn2.config(bg="black")
		btn3.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
		
	elif btn4["text"]=="x" and btn5["text"]=="x" and btn6["text"]=="x":
		btn4.config(bg="black")
		btn5.config(bg="black")
		btn6.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
		
	elif btn7["text"]=="x" and btn8["text"]=="x" and btn9["text"]=="x":
		btn7.config(bg="black")
		btn8.config(bg="black")
		btn9.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
		
	elif btn1["text"]=="x" and btn4["text"]=="x" and btn7["text"]=="x":
		btn1.config(bg="black")
		btn4.config(bg="black")
		btn7.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
		
	elif  btn2["text"]=="x" and btn5["text"]=="x" and btn8["text"]=="x":
		btn2.config(bg="black")
		btn5.config(bg="black")
		btn8.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
		
	elif  btn3["text"]=="x" and btn6["text"]=="x" and btn9["text"]=="x":
		btn3.config(bg="black")
		btn6.config(bg="black")
		btn9.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
		
	elif  btn1["text"]=="x" and btn5["text"]=="x" and btn9["text"]=="x":
		btn1.config(bg="black")
		btn5.config(bg="black")
		btn9.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
		
		
	elif  btn3["text"]=="x" and btn5["text"]=="x" and btn7["text"]=="x":
		btn3.config(bg="black")
		btn5.config(bg="black")
		btn7.config(bg="black")
		messagebox.showinfo("","x win!!")
		root.destroy()
	
	
	


global clicked


clicked = True

def click(b):
	
	global clicked
	if b["text"]=="" and  clicked == True:
		b["text"] = "o"
		clicked = False
		over()
		
	elif b["text"] =="" and clicked == False:
		b["text"] = "x"
		clicked = True
		over()
	else:
		messagebox.showinfo("","That box already selected")

	
btn1=Button(root,text="",width=10,height=10,command=lambda: click(btn1))
btn2=Button(root,text="",width=10,height=10,command=lambda: click(btn2))
btn3=Button(root,text="",width=10,height=10,command=lambda: click(btn3))
btn4=Button(root,text="",width=10,height=10,command=lambda: click(btn4))
btn5=Button(root,text="",width=10,height=10,command=lambda: click(btn5))
btn6=Button(root,text="",width=10,height=10,command=lambda: click(btn6))
btn7=Button(root,text="",width=10,height=10,command=lambda: click(btn7))
btn8=Button(root,text="",width=10,height=10,command=lambda: click(btn8))
btn9=Button(root,text="",width=10,height=10,command=lambda: click(btn9))

btn1.grid(column=0,row=0)
btn2.grid(column=1,row=0)
btn3.grid(column=2,row=0)
btn4.grid(column=0,row=1)
btn5.grid(column=1,row=1)

btn6.grid(column=2,row=1)
btn7.grid(column=0,row=2)
btn8.grid(column=1,row=2)
btn9.grid(column=2,row=2)


root.mainloop()
