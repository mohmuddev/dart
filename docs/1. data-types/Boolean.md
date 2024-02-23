---
sidebar_position: 3
---

# Boolean Data Type

### 1. Boolean Data Type:

In Dart, the boolean data type represents two values: `true` and `false`. It's used to express logical states, such as whether a condition is true or false.

#### Example:
```Javascript
bool isRaining = true;
bool isSunny = false;
```

### 2. Comparison Operators:

Comparison operators are used to compare values. They return a boolean value (`true` or `false`) based on the comparison result.

- `==` : Equal to
- `!=` : Not equal to
- `>`  : Greater than
- `<`  : Less than
- `>=` : Greater than or equal to
- `<=` : Less than or equal to

#### Example:
```Javascript
int a = 10;
int b = 5;

print(a == b); // false
print(a != b); // true
print(a > b);  // true
print(a < b);  // false
print(a >= b); // true
print(a <= b); // false
```

### 3. Logical Operators:

Logical operators are used to combine boolean expressions. Dart supports three logical operators:

- `&&` : Logical AND
- `||` : Logical OR
- `!`  : Logical NOT

#### Example:
```Javascript
bool isSunny = true;
bool isWarm = false;

// Logical AND
bool goOutside = isSunny && isWarm;
print(goOutside); // false

// Logical OR
bool goForWalk = isSunny || isWarm;
print(goForWalk); // true

// Logical NOT
bool stayInside = !goOutside;
print(stayInside); // true
```

### 4. Conditional Operators:

Conditional operators are used to simplify conditional expressions. Dart has a conditional operator (`? :`) which is often referred to as the ternary operator.

#### Example:
```Javascript
int age = 20;
String status = (age >= 18) ? 'Adult' : 'Minor';
print(status); // Adult
```
