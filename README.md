# Containers
Implementation of C++ STL containers library

---

## List of implemented containers and short description

- deque - Double ended queue. Based on dynamic array of pointers. Each pointer is responsible for 32-elements chunk.
- queue - Adapter on deque. Implements the FIFO principle.
- stack - Adapter on queue. Implements the LIFO principle.
- vector - Dynamic array. Every time the number of elements reaches the maximum capacity the array grows twice.
- list - Linked list. Nodes contain elements and have references on next and previous nodes.
- map - Container that holds unique elements in pair of key and value. Based on AVL tree.
- set - Container that holds unique elements. Every element plays role of key. Based on AVL tree.
- multiset - Set, but may contain not only unique elements. Based on the AVL tree.

## Run tests
To build and run tests:\
```cd src && make test```\
You can also see tests coverage:\
```cd src && make gcov_report```

## Usage
```// example.cpp
#include "s21_containers.h"

int main() {
  s21::vector<int> exampleVector = {1, 2, 3, 4};
  s21::deque<float> exampleDeque;
  exampleDeque.push_front(1.0f);
  exampleDeque.push_back(2.0f);
  return 0; 
}
