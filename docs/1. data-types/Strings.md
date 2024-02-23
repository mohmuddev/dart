---
sidebar_position: 2
---

# Strings Data Type

### 1. Creating Strings:

```JavaScript
String singleQuotedString = 'This is a single-quoted string';
String doubleQuotedString = "This is a double-quoted string";
```

### 2. String Interpolation:

String interpolation allows you to embed expressions within a string.

```JavaScript
String name = 'Alice';
int age = 30;
String greeting = 'My name is $name and I am $age years old.';
print(greeting); // Output: My name is Alice and I am 30 years old.
```

### 3. Escaping Characters:

You can escape characters using a backslash (\) in Dart strings.

```JavaScript
String stringWithEscapes = 'This is a \'single-quoted\' string';
print(stringWithEscapes); // Output: This is a 'single-quoted' string
```

### 4. Multiline Strings:

Dart supports multiline strings using triple quotes (''' or """).

```JavaScript
String multilineString = '''
  This is a
  multiline
  string
''';
print(multilineString);
```

### 5. Concatenating Strings:

You can concatenate strings using the '+' operator.

```JavaScript
String str1 = 'Hello';
String str2 = ' World';
String concatenatedString = str1 + str2;
print(concatenatedString); // Output: Hello World
```

### 6. String Length:

You can get the length of a string using the `length` property.

```JavaScript
String str = 'Hello';
print(str.length); // Output: 5
```

### 7. Converting to Uppercase/Lowercase:

You can convert strings to uppercase or lowercase using `toUpperCase()` and `toLowerCase()` methods.

```JavaScript
String str = 'Hello';
print(str.toUpperCase()); // Output: HELLO
print(str.toLowerCase()); // Output: hello
```

### 8. Substring:

You can extract a substring using the `substring()` method.

```JavaScript
String str = 'Dart Programming';
print(str.substring(5)); // Output: Programming
print(str.substring(5, 10)); // Output: Progr
```

### 9. Searching within Strings:

You can search for substrings within strings using `contains()`, `startsWith()`, and `endsWith()` methods.

```dart
String str = 'Dart Programming';
print(str.contains('Prog')); // Output: true
print(str.startsWith('Dart')); // Output: true
print(str.endsWith('ing')); // Output: true
```

### 10. Splitting Strings:

You can split a string into a list of substrings using `split()` method.

```JavaScript
String str = 'Hello World';
List<String> parts = str.split(' ');
print(parts); // Output: [Hello, World]
```

### 11. Trimming Strings:

You can remove leading and trailing whitespace from a string using the `trim()`, `trimLeft()`, and `trimRight()` methods.

```JavaScript
String str = '   Hello   ';
print(str.trim()); // Output: Hello
print(str.trimLeft()); // Output: Hello   
print(str.trimRight()); // Output:    Hello
```

### 12. Checking Empty Strings:

You can check if a string is empty using the `isEmpty` property.

```JavaScript
String str1 = '';
String str2 = 'Hello';
print(str1.isEmpty); // Output: true
print(str2.isEmpty); // Output: false
```

### 13. Replacing Substrings:

You can replace substrings within a string using the `replaceFirst()` or `replaceAll()` methods.

```JavaScript
String str = 'Hello World';
print(str.replaceFirst('Hello', 'Hi')); // Output: Hi World
print(str.replaceAll('o', '0')); // Output: Hell0 W0rld
```

### 14. Checking Equality:

You can check if two strings are equal using the `==` operator.

```JavaScript
String str1 = 'Hello';
String str2 = 'World';
String str3 = 'Hello';
print(str1 == str2); // Output: false
print(str1 == str3); // Output: true
```

### 15. Converting to/from Integer:

You can convert strings to integers using `int.parse()` and integers to strings using `toString()` method.

```JavaScript
String str = '123';
int num = int.parse(str);
print(num); // Output: 123

int num = 456;
String str = num.toString();
print(str); // Output: 456
```

### 16. Checking Substring:

You can check if a string contains a substring using `indexOf()` method.

```JavaScript
String str = 'Dart Programming';
print(str.indexOf('Pro')); // Output: 5 (index of the substring)
print(str.indexOf('JavaScript')); // Output: -1 (if substring not found)
```

### 17. Formatting Strings:

You can format strings using `printf`-style formatting.

```JavaScript
String name = 'Alice';
int age = 30;
String formattedString = 'My name is %s and I am %d years old.'.printf([name, age]);
print(formattedString); // Output: My name is Alice and I am 30 years old.
```

