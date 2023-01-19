# overlay
how to make overlay using tkinter 




#### The code

```python
from tkinter import *

root=Tk()

root.title("overlay")

x="0"
y="0"

root.geometry(f'250x150+{x}+{y}')
# to remove the titalbar 
root.overrideredirect(True)

# to make the window transparent  
root.attributes("-transparentcolor","red")
# set bg to red in order to make it transparent
root.config(bg="red")



l=Label(root,text="HI this is an overlay",fg="white",font=(60),bg="red")
l.pack()

b=Button(root,text="click me to print somthing",command=lambda:print("this is something"))
b.pack()

#make window to be always on top 
root.wm_attributes("-topmost", 1) 


root.mainloop()
```

The co-ordinates where the window should open.
```
x="0"
y="0"

root.geometry(f'250x150+{x}+{y}')
```

This remove the titalbar from the UI and icon from taskbar
```
# to remove the titalbar 
root.overrideredirect(True)

```
This is how to make the window transparent
```
root.attributes("-transparentcolor","red")
roo.config(bg="red")
```

