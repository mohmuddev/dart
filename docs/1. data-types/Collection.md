---
sidebar_position: 5
---

# Collection Data Types

### 1. Lists

```Javascript
// Creating a list
List<int> numbers = [1, 2, 3, 4, 5];

// Adding elements
numbers.add(6); // Adds a single element
numbers.addAll([7, 8, 9]); // Adds multiple elements

// Removing elements
numbers.remove(3); // Removes the first occurrence of specified value
numbers.removeAt(0); // Removes element at specified index
numbers.removeLast(); // Removes the last element
numbers.removeWhere((element) => element % 2 == 0); // Removes elements based on condition
numbers.clear(); // Removes all elements

// Accessing elements
int firstElement = numbers.first; // Access the first element
int lastElement = numbers.last; // Access the last element
int elementAtIndex = numbers[2]; // Access element at index

// Modifying elements
numbers[0] = 10; // Modify element at index 0

// Checking for element existence
bool contains = numbers.contains(5); // Checks if the list contains the specified value

// Sorting
numbers.sort(); // Sorts the list

// Iterating through elements
numbers.forEach((element) {
  // Perform an operation on each element
});

// Length of the list
int length = numbers.length; // Get the length of the list
```

### 2. Sets

```Javascript
// Creating a set
Set<int> numbersSet = {1, 2, 3, 4, 5};

// Adding elements
numbersSet.add(6); // Adds a single element
numbersSet.addAll([7, 8, 9]); // Adds multiple elements

// Removing elements
numbersSet.remove(3); // Removes the specified value
numbersSet.clear(); // Removes all elements

// Accessing elements
// Sets do not have direct access to elements by index

// Checking for element existence
bool contains = numbersSet.contains(5); // Checks if the set contains the specified value

// Iterating through elements
numbersSet.forEach((element) {
  // Perform an operation on each element
});

// Length of the set
int length = numbersSet.length; // Get the number of elements in the set
```

### 3. Maps

```Javascript
// Creating a map
Map<String, int> ages = {
  'John': 30,
  'Alice': 25,
  'Bob': 35,
};

// Adding elements
ages['Charlie'] = 40; // Adds a single key-value pair

// Removing elements
ages.remove('Alice'); // Removes the key-value pair with the specified key
ages.clear(); // Removes all key-value pairs

// Accessing elements
int johnsAge = ages['John']; // Access value by key

// Checking for element existence
bool containsKey = ages.containsKey('Alice'); // Checks if the map contains the specified key
bool containsValue = ages.containsValue(25); // Checks if the map contains the specified value

// Iterating through elements
ages.forEach((key, value) {
  // Perform an operation on each key-value pair
});

// Length of the map
int length = ages.length; // Get the number of key-value pairs in the map
```

