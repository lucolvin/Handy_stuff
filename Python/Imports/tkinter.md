`import tkinter` in Python is used to create graphical user interfaces (GUIs). The `tkinter` module provides a set of tools and widgets that allow developers to build interactive and visually appealing applications. Here are some common uses of `import tkinter`:

1. **Window Creation:** The primary use of `tkinter` is to create the main application window. Developers can use the `Tk` class to instantiate a top-level window where the GUI components will be placed.

   ```python
   import tkinter as tk

   root = tk.Tk()  # creates the main window
   ```

2. **Widgets:** `tkinter` provides a variety of widgets such as buttons, labels, entry fields, text boxes, and more. These widgets are used to create different elements in the GUI.

   ```python
   button = tk.Button(root, text="Click me", command=callback)
   label = tk.Label(root, text="Hello, Tkinter!")
   entry = tk.Entry(root)
   ```

3. **Event Handling:** With `tkinter`, you can define functions (callbacks) that are triggered in response to events like button clicks or key presses.

   ```python
   def button_click():
       print("Button clicked!")

   button = tk.Button(root, text="Click me", command=button_click)
   ```

4. **Layout Management:** `tkinter` provides different layout managers (pack, grid, and place) to arrange widgets in the application window. This allows for the creation of complex and organized GUIs.

   ```python
   button1 = tk.Button(root, text="Button 1")
   button2 = tk.Button(root, text="Button 2")

   button1.pack(side=tk.LEFT)
   button2.pack(side=tk.RIGHT)
   ```

5. **Dialog Boxes:** `tkinter` includes pre-built dialog boxes for common tasks such as file selection, color selection, and message boxes.

   ```python
   from tkinter import filedialog

   file_path = filedialog.askopenfilename()
   ```

6. **Canvas Drawing:** `tkinter` provides a `Canvas` widget that allows for drawing shapes, lines, and images.

   ```python
   canvas = tk.Canvas(root, width=200, height=200)
   canvas.create_line(0, 0, 200, 200)
   ```

7. **Menu Creation:** `tkinter` enables the creation of menus and menu bars for navigation and user interaction.

   ```python
   menu_bar = tk.Menu(root)
   root.config(menu=menu_bar)

   file_menu = tk.Menu(menu_bar, tearoff=0)
   menu_bar.add_cascade(label="File", menu=file_menu)
   ```
