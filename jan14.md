# Jan 14 Notes

 - We are leaning how to do time complexity, which is essential for algorthmic analysis

## Detect Duplicates

- We learned that one approach for finding duplicates is using two for loops, so that would be n^2 time complexity
- Another approach is using a hashmap, C doesnt include a hashmap in the standard library

## Compiling C Programs

Header file -> source file -> compile -> object file -> link -> exectuable file
foo.h       ->    foo.c    ->  gcc -c ->   foo.o     ->   gcc ->  foo

### Makefiles
- Makefiles consist of a set of rules for actions to compile **targets** from their **sources**
- Internally, make constructs a directed acyclic graph (DAG, a data structure!) from the rules
- make then preforms a topological sort of the DAG to determining the order in which to process the rules
  
### Testing for correctness: **assert**
- assert(condition)
- Keeps going if condition is true
- exits program with an error code and prints error message if the condition is false
- this is used to write unit tests
