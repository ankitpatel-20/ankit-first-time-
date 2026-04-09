#GUI Programming
    #web based(html/css/js/bootstrap,etc.)------>runs on browser
    #desktop based(tkinter,pyqt,wxpython,etc.)-->runs as independent window

#tkinter-->standard python library to create desktop based gui applications

from tkinter import Tk
root=Tk()                                   #create top level window
#root.geometry("500x300")                   #initial width x height
root.state("zoomed")                        #fullscreen window
root.resizable(width=False,height=False)    #disable resizing at runtime
root.configure(bg="yellow")                 #background of window
root.mainloop()                             #display the window

print(--------------------------------------------------------------------------------------------------------------------------------------------------------)

from tkinter import Tk,Button
root=Tk()                                   
root.geometry("500x300")                                      
root.configure(bg="yellow")

b1=Button(root,text="submit")
b2=Button(root,text="ok")

b1.place(x=100,y=100)
b2.place(x=300,y=100)

root.mainloop()                            
print(--------------------------------------------------------------------------------------------------------------------------------------------------------)

from tkinter import Tk,Button
root=Tk()                                   
root.geometry("500x300")                                      
root.configure(bg="yellow")

b1=Button(root,text="submit",width=7,font=('arial',15,'bold'),bd=5,bg='purple',fg='white')
b2=Button(root,text="ok",width=7,font=('arial',15,'bold'),bd=5)

#absolute
b1.place(x=100,y=100)
b2.place(x=300,y=100)

root.mainloop()                            

print(--------------------------------------------------------------------------------------------------------------------------------------------------------)

from tkinter import Tk,Button
root=Tk()                                   
root.geometry("500x300")                                      
root.configure(bg="yellow")

b1=Button(root,text="submit",width=7,font=('arial',15,'bold'),bd=5,bg='purple',fg='white')
b2=Button(root,text="ok",width=7,font=('arial',15,'bold'),bd=5)

#relative
b1.place(relx=.2,rely=.3)
b2.place(relx=.5,rely=.3)

root.mainloop()                            

print(--------------------------------------------------------------------------------------------------------------------------------------------------------)

from tkinter import Tk,Button
root=Tk()                                   
root.geometry("500x300")                                      
root.configure(bg="yellow")

b1=Button(root,text="submit",width=7,font=('arial',15,'bold'),bd=5,bg='purple',fg='white')
b2=Button(root,text="ok",width=7,font=('arial',15,'bold'),bd=5)

b1.pack(side="bottom",anchor='c')
b2.pack() #top,c

root.mainloop()                            



