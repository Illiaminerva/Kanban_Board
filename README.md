Link to the screen recording: https://www.loom.com/share/b630e77d9562431c901e0d3e9dabb3d1
Due to unforeseen circumstances, my local machine couldn't import the necessary libraries. Thus, I decided to do my project on repl.it (as you can see from the recording). Except for files, I am also attaching the link to my repl.it project here, so you can run it on your device:

Link: https://replit.com/@Illiaminerva/KanbanBoard#main.py

I sincerely apologize for such inconvenience.

The overall idea of this project is to create a Kanban board where people can put their tasks. On the website, users are able to take such actions:

- With button, create a new task that will automatically be added to the "Todo" list

- Move the task from "Todo" list to "Doing" list.

- Move the task from "Doing" list to "Done" list.

- Delete the task from "Todo" list.

- Delete the task from "Doing" list.

- Delete the task from "Done" list.

- Based on these features, the user is able to create their own tasks, move them from one column to another, and delete them in case they don't need to be accomplished anymore. 

- In order to work properly, this project contains several files. The main one is main.py, where the general Python code for my project is written. However, it will only be working with index.html file, where the HTML code is written, and the CSS file style.css, where styling is created. The style.css file is located in the folder static, while index.html is located in the templates folder. It doesn't make much of a difference for this small project, but for larger ones, it is crucial to separate the main Python file, the HTML files, and the CSS files.

Here are routes that exist in main.py file:

@app.route("/") – Initial Kanban board for a user, with a few sample tasks putten there

@app.route("/move_to_doing/<int:index>," methods=["POST"]) – A route that corresponds to the button for moving a task from "todo" column to "doing" column. 

@app.route("/move_to_done/<int:index>", methods=["POST"]) – A route that corresponds to the button for moving a task from the "doing" to the "done" column.

@app.route("/add", methods=["POST"]) – A route that corresponds to the button adding a task to "todo" list.

@app.route("/delete_todo/<int:index>") – A route that corresponds to the button deleting a task from todo list.

@app.route("/delete_todo/<int:index>") – A route that corresponds to the button deleting a task from todo list.

@app.route("/delete_doing/<int:index>") – A route that corresponds to the button deleting a task from doing list.

@app.route("/delete_done/<int:index>") – A route that corresponds to the button deleting a task from done list.
