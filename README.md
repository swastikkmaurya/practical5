# practical5
Aim : Study Of Python Dictionaries

Theory : 
A Python dictionary is a built-in mapping type that allows you to store data in key-value pairs, creating a relationship between a unique identifier (the key) and its associated data (the value). Unlike sequences like lists or tuples, which are indexed by a range of numbers, dictionaries are indexed by keys. These keys must be of an immutable (unchangeable) data type, such as strings, numbers, or tuples. This structure is modeled after a real-world dictionary where you look up a "word" (the key) to find its "definition" (the value). One of the most critical aspects of a dictionary is its efficiency; it uses a process called hashing to look up data, which means that finding a value takes roughly the same amount of time regardless of whether the dictionary has ten items.
Key Properties and Behavior

One of the most defining characteristics of a dictionary is that keys must be unique. As you demonstrated in your Ford example, if you attempt to assign a value to a key that already exists, Python doesn't throw an error; instead, it simply overwrites the old value with the new one. This makes dictionaries "latest-value" biased. Regarding order, it is important to note that while older versions of Python treated dictionaries as unordered, modern Python guarantees that dictionaries maintain the insertion order. This means that when you iterate through a dictionary, the items will appear in the exact order you added them. However, they remain mutable, meaning you can grow, shrink, or modify them in place without creating a new object in memory, which is why your product price update worked so seamlessly.

Python dictionaries implement hash tables using open addressing with linear probing, providing average O(1) lookup, insertion, and deletion regardless of size. Each key generates a hash value via  hash(key)  that maps to table indices; collisions are resolved deterministically, ensuring consistent access speeds critical for real-time embedded systems like Arduino data logging.

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
