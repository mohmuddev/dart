---
sidebar_position: 1
---

# Numeric Data Types
In Dart, there are mainly two types of numbers:

1. **Integers (`int`)**: Integers represent whole numbers without any fractional or decimal part. They can be positive, negative, or zero.

2. **Floating-Point Numbers (`double`)**: Floating-point numbers represent numbers that have a fractional part, i.e., they can hold decimal points. They can also be positive, negative, or zero.

Now, let's delve into each type in more detail and explore some common operations and methods associated with them.

### Integers (`int`):

1. **Initialization**: You can initialize an integer variable like this:
   ```dart
   int myInteger = 10;
   ```

2. **Arithmetic Operations**: You can perform basic arithmetic operations like addition, subtraction, multiplication, and division:
   ```javascript
   int a = 10;
   int b = 5;
   int sum = a + b; // 15
   int difference = a - b; // 5
   int product = a * b; // 50
   int quotient = a ~/ b; // 2 (integer division, discards remainder)
   ```

3. **Common Methods**:
   - `abs()`: Returns the absolute value of the integer.
   - `isEven`: Returns true if the integer is even.
   - `isOdd`: Returns true if the integer is odd.
   - `toString()`: Converts the integer to a string.
   - `compareTo()`: Compares two integers.


    1. **abs()**: 
        - Syntax: `int.abs()`
        - Description: Returns the absolute (non-negative) value of the integer.
        - Example:
            ```javascript
            int num = -10;
            int absValue = num.abs(); // absValue will be 10
            ```

    2. **isEven**:
        - Syntax: `int.isEven`
        - Description: Returns `true` if the integer is even, `false` otherwise.
        - Example:
            ```javascript
            int num = 10;
            bool isEvenNumber = num.isEven; // isEvenNumber will be true
            ```

    3. **isOdd**:
        - Syntax: `int.isOdd`
        - Description: Returns `true` if the integer is odd, `false` otherwise.
        - Example:
            ```javascript
            int num = 11;
            bool isOddNumber = num.isOdd; // isOddNumber will be true
            ```

    4. **toString()**:
        - Syntax: `int.toString()`
        - Description: Converts the integer to its string representation.
        - Example:
            ```javascript
            int num = 123;
            String strNum = num.toString(); // strNum will be "123"
            ```

    5. **compareTo()**:
        - Syntax: `int.compareTo(other)`
        - Description: Compares this integer to the given integer `other`. Returns a negative value if this integer is less than `other`, zero if they are equal, and a positive value if this integer is greater than `other`.
        - Example:
            ```javascript
            int num1 = 10;
            int num2 = 5;
            int result = num1.compareTo(num2); // result will be 1
            // Since num1 > num2, compareTo() returns a positive value (1)
            ```


### Floating-Point Numbers (`double`):

1. **Initialization**: You can initialize a double variable like this:
   ```dart
   double myDouble = 3.14;
   ```

2. **Arithmetic Operations**: You can perform arithmetic operations similar to integers:
   ```dart
   double x = 3.5;
   double y = 2.0;
   double sum = x + y; // 5.5
   double product = x * y; // 7.0
   double quotient = x / y; // 1.75
   ```

3. **Common Methods**:
   - `abs()`: Returns the absolute value of the double.
   - `ceil()`: Returns the smallest integer greater than or equal to the double.
   - `floor()`: Returns the largest integer less than or equal to the double.
   - `round()`: Rounds the double to the nearest integer.
   - `toStringAsFixed()`: Converts the double to a string with a specified number of decimal places.


    1. **abs()**: 
        - Syntax: `double.abs()`
        - Description: Returns the absolute (non-negative) value of the double.
        - Example:
            ```javascript
            double num = -3.14;
            double absValue = num.abs(); // absValue will be 3.14
            ```

    2. **ceil()**:
        - Syntax: `double.ceil()`
        - Description: Returns the smallest integer greater than or equal to the double.
        - Example:
            ```javascript
            double num = 3.14;
            double ceiledValue = num.ceil(); // ceiledValue will be 4.0
            ```

    3. **floor()**:
        - Syntax: `double.floor()`
        - Description: Returns the largest integer less than or equal to the double.
        - Example:
            ```javascript
            double num = 3.14;
            double flooredValue = num.floor(); // flooredValue will be 3.0
            ```

    4. **round()**:
        - Syntax: `double.round()`
        - Description: Rounds the double to the nearest integer.
        - Example:
            ```javascript
            double num = 3.5;
            double roundedValue = num.round(); // roundedValue will be 4.0
            ```

    5. **toStringAsFixed()**:
        - Syntax: `double.toStringAsFixed(n)`
        - Description: Converts the double to a string with a specified number of decimal places (`n`).
        - Example:
            ```javascript
            double num = 3.14159;
            String strNum = num.toStringAsFixed(2); // strNum will be "3.14"
            // It rounds to two decimal places
            ```

