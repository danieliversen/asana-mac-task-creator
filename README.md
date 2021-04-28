# Asana Quick Task Creator App for Mac

A small Apple MacOS Automator script to create Asana tasks quickly. The script results in a small app you can quickly bring up when creating a task. The tasks are assigned to yourself (but you can change that in the script) which results them being placed in your My Task list.


## Steps to install

1. Open Automator app
2. Create new app
3. Paste in code from the repository
4. Add your [Asana API Token](https://www.youtube.com/watch?v=AubkOn_-VBE)
5. Save app
6. Change icon if neccessary


## How to use app
Open app or use Spotlight for quick access:

<img width="480" alt="Screen Shot 2021-04-28 at 4 25 10 pm" src="https://user-images.githubusercontent.com/1035157/116356359-8358b680-a83e-11eb-97a4-7fbaeba0f777.png">


Enter task details and press ok:

<img width="420" alt="Screen Shot 2021-04-28 at 4 24 28 pm" src="https://user-images.githubusercontent.com/1035157/116356377-894e9780-a83e-11eb-92ec-c3ce89651a55.png">

The task will end up in your Asana "My Task" list


## How to change the task details

### Adding a tag
If you wanted to add a tag to a task while creating it, just edit the Automator script and add the following to the curl command (substituting the ID with your desired tag ID):
```
--data-urlencode \"tags=1200257943766397\" 
```

### Adding the task to a project
If you want to add the task directly into a project (it will still be in your My Tasks as long as it's assigned to you), add the following to the curl command in the script (substituting the ID with your desired target project ID):
--data-urlencode \"projects=1180040680315281\"
