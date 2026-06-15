# Territory War Simulator in C

A C programming project that simulates a territory-based strategy game while demonstrating core software engineering and data structure concepts.

## Features

* Territory management using arrays of structures (`Territory`)
* Territory attack system using pointers and dynamic memory allocation
* Strategic mission system implemented with function pointers
* Troop movement between territories
* Dynamic neighborhood relationships between territories
* Win-condition verification through customizable mission logic

## Project Structure

```text
.
├── main.c
├── territory.c
├── territory.h
├── attack.c
├── attack.h
├── mission.c
├── mission.h
└── Makefile
```

## Technical Concepts Demonstrated

* Structures (`struct`)
* Pointers
* Dynamic memory allocation (`malloc`, `realloc`, `free`)
* Function pointers
* Modular software design
* Game state management
* Memory lifecycle management

## Build

```bash
make
```

## Run

```bash
./war
```

## Terminal Controls

| Command | Description                        |
| ------- | ---------------------------------- |
| 1       | Display map                        |
| 2       | Attack a territory (`fromId toId`) |
| 3       | Move troops (`fromId toId qty`)    |
| -1      | Exit the game                      |

## Sample Scenario

The default mission requires a player to control at least **four territories**.

The sample map contains:

* 6 territories
* 2 players (Player 0 and Player 1)

## Memory Management

The project demonstrates explicit memory management in C:

* Territory names and colors are dynamically allocated using `malloc`
* Territory neighbor lists are dynamically expanded using `realloc`
* Mission objects are allocated dynamically and released during cleanup
* All allocated resources are properly released before program termination

## Learning Objectives

This project was developed to practice:

* Data structures in C
* Dynamic memory management
* Pointer manipulation
* Function pointer usage
* Modular architecture
* Strategy game simulation concepts

## License

MIT License
