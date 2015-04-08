# stacktracker
A stack-based (anti)productivity tracker tool.

### Idea
The idea of stacktracker is to provide a simple way of keeping track of things you are doing, by allowing you to push a new task onto the stack as you are invariably interrupted during the day.

### Commands
Three commands are provided, ```push```, ```pop``` and ```stack```. ```push``` takes the name of a task as an argument, and pushes it to the stack. ```pop``` removes the top task from the stack and prints it. ```stack``` shows the entire stack.

The stack is stored in the file ```~/.stack```, and the file ```~/.stacktmp``` is used as temporary storage. In a future version, the storage file may be made configurable via environment variable.

### Implementation
stacktracker is implemented as three minimal (or at least quite short) bash scripts.

### Examples

```
➜  push "Write README.md"
➜  push "Make coffee"
➜  stack
Make coffee
Write README.md
➜  pop
Pop'd Make coffee
➜  pop
Pop'd Write README.md
```
