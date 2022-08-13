# SUMIT-SETH
#This is for beginners programmer "Make a simple calculator on GUI BASED."

from tkinter import*
win=Tk()
win.geometry('300x100')
win.title('Simple Calculator by sumit')
#functions
def add():
 x=int(n1.get())
 y=int(n2.get())
 res=x+y
 lblres.config(text=str(x)+'+'+str(y)+'='+str(res))

def sub():
 x=int(n1.get())
 y=int(n2.get())
 res=x-y
 lblres.config(text=str(x)+'-'+str(y)+'='+str(res))

def mult():
 x=int(n1.get())
 y=int(n2.get())
 res=x*y
 lblres.config(text=str(x)+'*'+str(y)+'='+str(res))

def div():
 x=int(n1.get())
 y=int(n2.get())
 res=x/y
 lblres.config(text=str(x)+'/'+str(y)+'='+str(res))

#Label
lbln1=Label(win,text='Enter First No',fg='blue',font=('arial',20))
lbln1.place(x=50,y=50)
lbln2=Label(win,text='Enter Second No',fg='blue',font=('arial',20))
lbln2.place(x=50,y=100)
lblres=Label(win,text='Result',fg='blue',font=('arial',20))
lblres.place(x=50,y=150)
#Entry
n1=StringVar()
entn1=Entry(win,bg='red',fg='white',font=('arial',20),textvariable=n1,bd=5)
entn1.place(x=270,y=50)
n2=StringVar()
entn2=Entry(win,bg='red',fg='white',font=('arial',20),textvariable=n2,bd=5)
entn2.place(x=270,y=100)

#Button
btnadd=Button(win,text='Add',fg='blue',font=('arial',15),command=add)
btnadd.place(x=50,y=200)

btnsub=Button(win,text='Sub',fg='blue',font=('arial',15),command=sub)
btnsub.place(x=150,y=200)

btnmult=Button(win,text='Mult',fg='blue',font=('arial',15),command=mult)
btnmult.place(x=250,y=200)

btndiv=Button(win,text='Div',fg='blue',font=('arial',15),command=div)
btndiv.place(x=350,y=200)
win.mainloop()
