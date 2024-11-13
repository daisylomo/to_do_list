```python
#lists
"""
mutable data types(whose values can be altered)
square brackets
"""
#tuples
"""
immutable
normal brackets
"""
```




    '\nimmutable\nnormal brackets\n'




```python
tasks = []

while True:
    print("\n1. add \n2. delete \n3. view \n4. exit")
    choice = input("What do you want to do?")

    if choice == "1":
        task = input("Enter a task: ")
        if task in tasks:
            print("Task already included!")
        else:
            tasks.append(task)
            print("Success!")
            
    elif choice == "2":
        task = input("Which task? ")
        if task in tasks:
            tasks.remove(task)
            print("Success!")
        else:
            print("No such task!")
            
    elif choice == "3":
        print("TO-DO LIST")
        for i, task in enumerate(tasks, 1):
            print(f"{i}.{task}")
            
    elif choice == "4":
        print("Done!")
        break
        
    else:
        print("Error! Pick a number!")
```

    
    1. add 
    2. delete 
    3. view 
    4. exit
    

    What do you want to do? 2
    Which task?  rat sb out
    

    No such task!
    
    1. add 
    2. delete 
    3. view 
    4. exit
    

    What do you want to do? 1
    Enter a task:  race
    

    Success!
    
    1. add 
    2. delete 
    3. view 
    4. exit
    

    What do you want to do? 1
    Enter a task:  race
    

    Task already included!
    
    1. add 
    2. delete 
    3. view 
    4. exit
    

    What do you want to do? 3
    

    TO-DO LIST
    1.race
    
    1. add 
    2. delete 
    3. view 
    4. exit
    

#### tasks = []

while True:
    print("\n1. Add Task\n2. Remove Task\n3. View Tasks\n4. Exit")
    choice = input("Choose an option: ")

    if choice == "1":
        task = input("Enter a task: ")
        tasks.append(task)
        print(f"'{task}' added!")
    elif choice == "2":
        task = input("Enter the task to remove: ")
        if task in tasks:
            tasks.remove(task)
            print(f"'{task}' removed!")
        else:
            print("Task not found.")
    elif choice == "3":
        print("\nTo-Do List:")
        for i, task in enumerate(tasks, 1):
            print(f"{i}. {task}")
    elif choice == "4":
        print("Goodbye!")
        break
    else:
        print("Invalid choice. Try again.")



```python
tasks = []

while True:
    print("\n1. Add Task\n2. Remove Task\n3. View Tasks\n4. Exit")
    choice = input("Choose an option: ")
    
    if choice == "1":
        task = input("Enter a task: ")
        tasks.append(task)
        print(f"'{task}' added!")
        
    elif choice == "2":
        task = input("Enter the task to remove: ")
        if task in tasks:
            tasks.remove(task)
            print(f"'{task}' removed!")
        else:
            print("Task not found.")
            
    elif choice == "3":
        print("\nTo-Do List:")
        for i, task in enumerate(tasks, 1):
            print(f"{i}. {task}")
            
    elif choice == "4":
        print("Goodbye!")
        break
        
    else:
        print("Invalid choice. Try again.")

```

    
    1. Add Task
    2. Remove Task
    3. View Tasks
    4. Exit
    

    Choose an option:  exit
    

    Invalid choice. Try again.
    
    1. Add Task
    2. Remove Task
    3. View Tasks
    4. Exit
    

    Choose an option:  no
    

    Invalid choice. Try again.
    
    1. Add Task
    2. Remove Task
    3. View Tasks
    4. Exit
    

    Choose an option:  1
    Enter a task:  do
    

    'do' added!
    
    1. Add Task
    2. Remove Task
    3. View Tasks
    4. Exit
    

    Choose an option:  4
    

    Goodbye!
    


```python

```
