# todo
ToDo app written in Python

Clone:
------
git clone https://github.com/mlungwsr/todo.git

Run:
----
cd todo

./app.py

Access:
-------
List all tasks
--------------
curl -i -u sabelo:password http://localhost:5000/todo/api/v1.0/tasks

List single task
----------------
curl -i http://localhost:5000/todo/api/v1.0/tasks

Add a new task
--------------
curl -i -H "Content-Type: application/json" -X POST -d '{"title":"Elements of Freedom", "description": "One of the best Books ever!"}' http://localhost:5000/todo/api/v1.0/tasks

Update a task
-------------
curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2

Delete a task
-------------
curl -i -X DELETE  http://localhost:5000/todo/api/v1.0/tasks/2
