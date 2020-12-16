# Tkinter-Project

import tkinter
import tkinter.messagebox

class MyGUI:
    def __init__(self):
        self.main_window = tkinter.Tk()

        self.main_window.geometry('500x200')

        self.main_window.title('label demo')

        self.label1 = tkinter.Label(self.top_frame,text="This is the top frame")

        self.label2 = tkinter.Label(self.top_frame,text="This is also the top frame")

        seld.label3 = tkinter.label(self.top_frame,text = "this is also the top frame")

        self.label1.pack()
        self.label2.pack()
        self.label3.pack()

        self.label4 = tkinter.Label(self.bottom_frame,text="This is the bottom frame")

        self.label5 = tkinter.Label(self.bottom_frame,text="This is also the bottom frame")

        seld.label6 = tkinter.label(self.bottom_frame,text = "this is also the bottom frame")

        self.label4.pack(side='left')
        self.label5.pack(side='left')
        self.label6.pack(side='left')

        self.quit_button = tkinter.Button(self.main_window, text='Quit', command=self.main_window.destroy)
        self.my_button = tkinter.Button(self.main_window, text='click me', command=self.do_something)

        self.bottom_frame.pack()
        self.top_frame.pack()

        self.my_button.pack()
        self.quit_button.pack()

        tkinter.mainloop()
                                        
    def do_something(self):
        tkinter.messagebox.showinfo('Response','Thanks for clicking the button')

my_gui = MyGUI()

print("The End")
