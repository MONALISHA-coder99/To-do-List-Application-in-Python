# To-do-List-Application-in-Python
python project
tasks = []
def add_task(task):
   tasks.append(task)
   print(f"Task '{task}' added.")
def remove_task(task):
    if task in tasks:
        tasks.remove(task)
        print(f"Task '{task}' removed.")
    else:
        print(f"Tak '{task}' not found in the list.")
def show_tasks():
    if not tasks:
        print("No tasks in the list.")
    else:
      print("Tasks:")
      for index,task in enumerate(tasks):
          print(f"{index + 1}.{task}")
while True:
   print("\nTo-Do List Menu:")
   print("1. Add a task")
   print("2. Remove a task")
   print("3.Show tasks")
   print("4.Quit")

   choice = input("Enter  your choice: ")

   if choice == '1':
       task = input("Enter the task to add: ")
       add_task(task)
  elif choice == '2':
        task = input("Enter the task to remove: ")
        remove_task(task)
  elif choice == '3':
       show_tasks()
  elif choice == '4':
       print("Goodbye!)
       break
 else:
     print("Invalid choice.Please try again. ")



  
  
 
   
        

