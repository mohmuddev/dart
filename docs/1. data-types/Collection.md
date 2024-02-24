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

Absolutely! 

### 4. Enum

An enum, short for enumeration, is a special data type in programming that allows you to define a collection of related constant values. It's essentially a way to represent a fixed number of possible states or choices.

#### When to Use Enums?

You can use enums in situations where you have a predefined set of related constant values. Here are some common scenarios where enums are useful:

1. **Representing Options or Choices**: Enums are great for representing options or choices that have a fixed set of possible values. For example, days of the week, months of the year, colors, etc.

2. **State Management**: Enums are often used to represent states in an application. For instance, the different states of a user's session (logged in, logged out, idle) or the status of an approval process (pending, approved, rejected, canceled).

3. **Improving Readability and Maintainability**: Enums can make your code more readable and maintainable by giving meaningful names to the possible values of a variable. Instead of using arbitrary integers or strings to represent states, you can use descriptive enum constants.

Now, let's combine the explanation with the previous code example:

```javascript
// Define an enum for Approval Status
enum ApprovalStatus {
  pending,
  approved,
  rejected,
  canceled,
}

void main() {
  // Initialize a variable to store approval status
  ApprovalStatus status = ApprovalStatus.pending;

  // Simulating a change in status
  status = ApprovalStatus.approved;

  // Checking the status and performing actions accordingly
  switch (status) {
    case ApprovalStatus.pending:
      print('Approval is pending');
      break;
    case ApprovalStatus.approved:
      print('Approval has been granted');
      break;
    case ApprovalStatus.rejected:
      print('Approval has been rejected');
      break;
    case ApprovalStatus.canceled:
      print('Approval has been canceled');
      break;
  }
}
```

This code snippet now includes an explanation of what enums are and when to use them, along with the enum definition and usage example.

