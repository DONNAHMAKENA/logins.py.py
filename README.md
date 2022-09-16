# logins.py.py
from tkinter import *
from tkinter import messagebox
import ast

window=Tk()
window.title('login')
window.geometry('925*500+300+200')
window.configure(bg="#fff")
window.resizable(False,False)
 
def signin():
      username=user.get()
      password=code.get()
      confirm_password=confirm_code.get()


if password==confirm_password:
        try:
            file=open('datasheet.text','r+')
            d=file.read()
            r.ast.literal_eval(d)

        dict2={username:password}
        r.updates(dict2)
        file.truncate(0)
        file.close
        file=open('datasheet.txt','w')
        w=file.write(str(r))
    messagesbox.showinfo('signup','successfully signed up')

    
except:
      file=open('datasheet.txt','w')
      pp=str({'username':'password'})
      file.write(pp)
      file.close()

img=photoImage(file='imgres.html')                  
label=(window,image=img,bg='white').place(X=50,Y=50)
frame=frame(window,width=350,height=390,br="#fff")
frame.place(X=480,y=50)

heading=label(frame,text('sign up',fg='#57a1f8',bg='white',font='Microsoft YaHei UI Light',23,'bold'))
heading.place(X=100,Y=5)
########################----------------------------------
def 0n_enter(e):
  user.delete(0,'end')
  
def on_leave(e):
 if user.get==''
   user.insert(0,'Username')

user=Entry(frame,width=25,fg='black'border=0,bg='white',font='Microsoft YaHei UI Light',11))
user.place(X=30,Y=80)
user.insert(0,'Username')
user.bind=('<focusIn>',on_enter)
user.bind=('<focusIn>',on_leave)

frame(Frame,width=295,height=2,bg='black')
place(X=25,Y=107)

###############################################################---------------------
def 0n_enter(e):
code.delete(0,'end')

      def on_leave(e):
       name=code.get()
       ifname==''
             code.insert(0,'password')

code=entry(frame,width=25,fg='black'border=0,bg='white',font='Microsoft YaHei UI Light'
code.place=(X=30,Y=150)
code..insert(0,'Password')
code.bind=('<focusIn>',on_enter)
code.bind=('<focusIn>',on_leave)

frame(frame,width=295,height=2,bg='black').place(X=25,Y,1770

############################################################---------------------------
def 0n_enter(e):
code.delete(0,'end')

def on_leave(e):
       confirm_code.get()
       confirm_code.insert(0,'confirm password')

confirm_code=entry(frame,width=25,fg='black'border=0,bg='white',font='Microsoft YaHei UI Light'
confirm_code.place=(X=30,Y=150)
confirm_code..insert(0,' confirm Password')
confirm_code.bind=('<focusIn>',on_enter)
confirm_code.bind=('<focusIn>',on_leave)

frame(frame,width=295,height=2,bg='black').place(X=25,Y,1770


Button(frame,width=39,pady=7,text='sign in'text='sign in',bg='#57a1f8'fg='white',border=0,command=signin).place(X=35,Y=204)
label=label(frame,text="I have an account",fg='black',bg='white',font=('Microsoft YaHei UI Light')

sigin=button(framee,wifth=6,text='sign in',border=0,bg='white',cursor='hand2',fg='#57a1f8'
signin.place(X=200,Y=340)





root.mainloop()
