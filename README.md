# CODSOFT
todo_list=[]
while True:
    print("1. add task")
    print("2. view task")
    print("3. mark task as completed")
    print("4. exit")
    choice=int(input("enter your choice="))
    if(choice==1):
        task=input("enter a new task=")
        todo_list.append(task)
        print("task added successfully")
    elif(choice==2):
        print("tasks:")
        for index, task in enumerate(todo_list,start=1):
            print(f"{index}.{task}")
    elif(choice==3):
        task_index=int(input("enter the task number to mark it as completed="))
        if(task_index>=1 and task_index<=len(todo_list)):
            completed_task=todo_list.pop(task_index-1)
            print(f"task'{completed_task}' marked as completed")
    else:
        print("invalid choice, please try again")
