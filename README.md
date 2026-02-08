# practical5
Aim : Study Of Python Dictionaries

Theory : 
Python dictionaries efficiently store key-value pairs, as shown in your examples for products, students, and users. Your code demonstrates core operations like creation, updating, accessing, removing items, and finding maximum values using built-in methods.Dictionaries in Python are mutable, unordered collections of unique keys mapped to values, implemented as hash tables for O(1) average-time access. Keys must be immutable (e.g., strings, integers) and unique, while values can be any data type; duplicate keys overwrite prior values, as in your  year: 2020  example. Methods like  get(key, default) ,  pop(key) ,  values() ,  keys() , and  max(dict, key=dict.get)  enable safe retrieval, modification, deletion, iteration, and max-finding without errors for missing keys.Python dictionaries implement hash tables using open addressing with linear probing, providing average O(1) lookup, insertion, and deletion regardless of size. Each key generates a hash value via  hash(key)  that maps to table indices; collisions are resolved deterministically, ensuring consistent access speeds critical for real-time embedded systems like Arduino data logging.

Algorithm:
1.Creation:  dict = {key1: value1, key2: value2}  - Initialize with comma-separated key-value pairs.

2.Duplicate Key Overwrite:  dictkey = new_value  - Last assignment for duplicate key replaces previous value.

3.Length:  len(dict)  - Returns total number of key-value pairs.

4.Add/Update Item:  dictnew_key = value  - Assigns new key-value or updates existing key.

5.Access Value:  dictkey  or  dict.get(key, default)  - Retrieves value by key or safe default.

6.Access Name:  student"name"  - Direct bracket notation for key lookup.

7.Remove Item:  dict.pop(key)  - Deletes and returns value for specified key.

8.Update Product Price:  product"book" = 55  - Direct assignment overwrites existing price.

9.Search Student Marks:  marks.get(name, "Student not found")  - Safe lookup with default message.

10.Validate Login:  if users.get(username) == password: print("Welcome")  - Compare retrieved password with input.

11.Find Topper:  topper = max(marks, key=marks.get)  - Returns key with highest associated value.

Conclusion: These examples illustrate dictionaries’ power for real-world tasks like inventory updates, lookups, validation, and analytics, with methods ensuring robust, efficient code ideal for your ENTC projects. Practice by extending to nested dictionaries or loops for multiple toppers
