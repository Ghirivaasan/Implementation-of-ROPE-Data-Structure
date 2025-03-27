# Rope Data Structure Implementation

This C++ project implements a Rope data structure, which is an efficient way to store and manipulate large strings. The Rope data structure is particularly useful for text editing and processing applications where frequent insertions and deletions are required.

## Key Features

- **Efficient String Manipulation:** Allows for efficient insertion, deletion, and concatenation of strings.
- **Split Operation:** Splits the rope into two ropes at a specified index.
- **Concat Operation:** Concatenates two ropes into a single rope.
- **Insert Operation:** Inserts a string at a specified index within the rope.
- **Delete Operation:** Deletes a character at a specified index within the rope.
- **Menu-Driven Interface:** Provides a simple menu for users to interact with the Rope data structure.

## Installation

To use this project, you need a C++ compiler (e.g., g++) and a standard development environment.

1.  Clone the repository to your local machine.
2.  Compile the `main.cpp` file along with `rope.cpp` and `rope.h`.


## Usage

After compiling the code, you can run the executable. The program provides a menu-driven interface that allows you to perform various operations on the Rope data structure.


### Menu Options

1.  **Split**: Splits the rope into two ropes at a specified index.
2.  **Concat**: Concatenates the current rope with another rope.
3.  **Insert**: Inserts a string into the rope at a specified index.
4.  **Delete**: Deletes a character from the rope at a specified index.
5.  **Display**: Displays the contents of the rope.
6.  **Exit**: Exits the program.


## Code Structure

The project consists of the following files:

-   `rope.h`: Header file containing the declaration of the `Rope` class and its methods.
-   `rope.cpp`: Implementation file containing the definition of the `Rope` class methods.
-   `main.cpp`: Contains the main function that drives the menu-driven interface and tests the `Rope` data structure.

### Classes and Methods

#### Node Class

-   `Node(const string& str)`: Constructor to create a new node with the given string.
-   `string str`: The string stored in the node.
-   `Node* left`: Pointer to the left child node (not used in this implementation, but can be added for balanced trees).
-   `Node* right`: Pointer to the right child node.

#### Rope Class

-   `Rope()`: Default constructor to create an empty rope.
-   `Rope(const string& str)`: Constructor to create a rope with an initial string.
-   `void split(int index, Rope& left, Rope& right)`: Splits the rope into two ropes at the specified index. The left rope contains characters from the start to the index, and the right rope contains the remaining characters.
-   `void concat(const Rope& other)`: Concatenates the current rope with another rope.
-   `void insert(int index, const string& str)`: Inserts a string into the rope at the specified index.
-   `void deleteAt(int index)`: Deletes the character at the specified index from the rope.
-   `bool isEmpty() const`: Checks if the rope is empty.
-   `int length() const`: Returns the length of the rope.

### Helper Functions

-   `ostream& operator<<(ostream&, const Rope&)`: Overloads the output stream operator to display the contents of the rope.
-   `void display(const Rope& rope)`: Displays the contents of the rope.
-   `void printMenu()`: Displays the menu options.

## Contributing

Contributions are welcome! Please submit pull requests or issues to improve the code.

## License

This project is licensed under the MIT License.

