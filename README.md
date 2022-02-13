# AI Maze Solver
>Technology Used: **Pure Python**

>Built-in packages used: **sys** & **Image [PIL]**

AI based Maze Solver uses Stack or Queue Frontier's to encounter and solve maze's and helps you analyze which search problem has less path cost in similar scenarios. The program only uses uninformed search strategy since it's harder to analyse their behaviour. Program also generates an Image of the final result of the solved maze within the same as program directory with associated name *"maze.png"*. While giving the image output the user is also provided the option wether they want to see the explored path (path which was explored but did not result in provide to reach the goal.) or just the path that counts the actions which resulted in reaching the *Goal Point*. The program enumerates how many states were explored before reaching the goal using an reverse action algorithm which helps the user to analyze for which scenario which search problem type finds the optimal path.

4 distinct scenarios of maze's have been provided in the repo. User can create more in text files nevertheless it should be finite should exactly have **1 Start and 1 Goal Point.**


Preferably I use Queue Frontier but the user can always change between Breadth-First Search `QueueFrontier()` Class or Depth-First Search `StackFrontier` Class by editing the `frontier` variable
```
start = Node(state=self.start, parent=None, action=None)
frontier = StackFrontier()
frontier.add(start)
```
```
start = Node(state=self.start, parent=None, action=None)
frontier = QueueFrontier()
frontier.add(start)
```

## **Maze Legend**
![maze-legend](https://user-images.githubusercontent.com/67305606/153759315-f08e9b18-c94f-4c94-8548-239011c08af3.png)

## **Image Output**
After the maze is solved and the user provides the exploration argument an image with the name *maze.png* is printed and automatically opens the image before exiting the program.

![maze](https://user-images.githubusercontent.com/67305606/153759352-0f5618af-3879-44a0-b3d4-4389ac6c0486.png)

## Maze Output Legend
- ![#282828](https://via.placeholder.com/15/282828/000000?text=+) `Wall`
- ![#ff0000](https://via.placeholder.com/15/ff0000/000000?text=+) `Start Point`
- ![#00ab1c](https://via.placeholder.com/15/00ab1c/000000?text=+) `Goal Point`
- ![#dceb71](https://via.placeholder.com/15/dceb71/000000?text=+) `Goal Path`
- ![#d46155](https://via.placeholder.com/15/d46155/000000?text=+) `Explored Path`
- ![#edf0fc](https://via.placeholder.com/15/edf0fc/000000?text=+) `Blank Path`
