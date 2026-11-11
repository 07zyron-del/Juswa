# 📚 Library Management System

A library system built in Java for our 2nd-year OOP and Data Structures final project. It has a Java back end (`Library` and `LibraryServer`) and an HTML front end (`index.html`) where every button calls the Java code on the server.

## Features
- Add books, DVDs and magazines to the catalog
- Add library members
- Borrow, return and reserve items (with a waitlist when an item is already borrowed)
- Undo the last action
- Search by item ID or exact title
- View the catalog in different sort orders
- Activity log showing what happened

## Concepts Used
**OOP**
- Inheritance and abstraction: `LibraryItem` is the parent of `Book`, `DVD` and `Magazine`
- Encapsulation, polymorphism and interfaces: [check and edit]

**Data Structures**
- `HashMap`: stores items and members for fast lookup by ID
- Binary search tree (`TitleBST`): search and sorted view by title
- Sorting (`Sorter`): [name the algorithm, e.g. bubble sort or merge sort]
- Queue for waitlists, stack for undo: [check]

## Project Structure
| File | Purpose |
|---|---|
| `Library.java` | Main logic: borrow, return, reserve, undo |
| `LibraryItem.java`, `Book.java`, `DVD.java`, `Magazine.java` | Item classes |
| `Member.java` | Library member |
| `Action.java` | Records actions for undo |
| `TitleBST.java`, `Sorter.java` | Search and sorting |
| `LibraryServer.java` | Java server that the web page talks to |
| `index.html` | Web front end |
| `Main.java`, `LibraryGUI.java` | Console and desktop versions |
| `run.bat`, `run.sh` | Compile and start the server |

## How to Run
1. Install **Java JDK** [version, e.g. 17 or newer].
2. Download or clone this repository and extract it (don't run it from inside a zip).
3. Double-click **`run.bat`** (Windows) or run `./run.sh` (Mac/Linux). Or in a terminal:
   ```
   javac *.java
   java LibraryServer
   ```
4. Keep the terminal open, then open **`index.html`** in your browser.

## Try It
Maria borrows B01 → Juan reserves it → Maria returns it.

## Screenshots
*(add a screenshot of the web page here)*

## Authors
- [Your name] [and partner's name]
- Instructor: Joshua V. Porras
- Course: Object-Oriented Programming and Data Structures, [school], 2026
