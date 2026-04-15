
*This project has been created as part of the 42 curriculum by msimoes*
 
## Description
Push_Swap is a sorting algorithm project where a stack of integers must be sorted using only two stacks and a limited set of operations. The program receives a list of integers as arguments and outputs the sequence of operations needed to sort stack A in ascending order.
 
The goal of this project is to learn about algorithm complexity, optimization, and data structures by implementing an efficient sorting solution. The program uses the Turkish algorithm for larger sets, with dedicated handlers for small sets of 2, 3, 4, and 5 elements.
 
## Instructions
 
### Compilation
To compile the project simply run:
```bash
make
```
To recompile everything run:
```bash
make re
```
 
Both of these will create a `push_swap` executable.
 
### Usage
```bash
./push_swap [numbers]
```
 
### Arguments
- `[numbers]`: A list of unique integers to sort, passed as separate arguments or as a single quoted string
### Available Operations
| Operation | Description |
|-----------|-------------|
| `sa` | Swap the first two elements of stack A |
| `sb` | Swap the first two elements of stack B |
| `ss` | `sa` and `sb` at the same time |
| `pa` | Push the top of stack B onto stack A |
| `pb` | Push the top of stack A onto stack B |
| `ra` | Rotate stack A upward |
| `rb` | Rotate stack B upward |
| `rr` | `ra` and `rb` at the same time |
| `rra` | Reverse rotate stack A |
| `rrb` | Reverse rotate stack B |
| `rrr` | `rra` and `rrb` at the same time |
 
### Examples
Sort a list of numbers:
```bash
./push_swap 5 3 1 4 2
```
Count the number of operations:
```bash
./push_swap 5 3 1 4 2 | wc -l
```
Pass numbers as a string:
```bash
./push_swap "5 3 1 4 2"
```
 
### Cleanup
Remove object files:
```bash
make clean
```
Remove object files and executable:
```bash
make fclean
```
 
## Resources
- [Push_Swap tutorial - Medium](https://medium.com/@ayogun/push-swap-c1f5d2d41e97)
- [Turkish algorithm explanation](https://en.wikipedia.org/wiki/Sorting_algorithm)
- [Linked lists in C - GeeksForGeeks](https://www.geeksforgeeks.org/linked-list-in-c/)
- [Algorithm complexity - Wikipedia](https://en.wikipedia.org/wiki/Time_complexity)
### AI usage
No AI was used to write the code of this project. AI was only used to find problems with the code and suggest fixes.
It was also used to make a draft for the README.
