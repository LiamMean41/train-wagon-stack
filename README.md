# Java Stack ADT

A stack abstract data type (ADT) implemented from scratch in Java, with a train wagon-themed Swing GUI for interactive demonstration. Built as a college exercise to explore stack data structures and interface-driven design.

## How it works

The stack is backed by an `ArrayList` with index `0` as the top. A custom `StackInterface` defines the contract, and `MyStack` provides the concrete implementation.

| Interface method | Behaviour |
|---|---|
| `push(Object)` | Adds an item to the top of the stack |
| `remove()` | Pops and returns the top item (returns `null` if empty) |
| `add()` | Peeks at the top item without removing it |
| `get()` | Returns the top item |
| `getIndex(int)` | Returns the item at a given index |
| `size()` | Returns the number of items in the stack |
| `isEmpty()` | Returns true if the stack has no items |
| `displayStack()` | Returns all items as a formatted string |

## GUI features

The Swing interface frames the stack as a train wagon list:

- **Add Wagon** — pushes the text field input onto the stack
- **Remove Wagon** — pops the top wagon off the stack
- **Remove All Wagons** — clears the entire stack
- **List Wagons** — displays all wagons from top to bottom
- **Number of Wagons** — shows the current stack size
- **First Wagon** — retrieves the bottom item (first wagon added)

## Requirements

- Java 8 or higher
- NetBeans IDE (recommended — project includes `nbproject/` config)

## Getting started

Open in NetBeans via `File → Open Project` and run, or build manually:

```bash
javac -sourcepath src -d out src/stack2023/StackApp.java
java -cp out stack2023.StackApp
```

On launch, `StackApp` runs a console self-test (pushing Iron, Coal, and Dirt, then popping them) before opening the GUI window.
