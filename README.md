# practical5
Aim : Study Of Python Dictionaries

Theory : 
A Python dictionary is a built-in mapping type that allows you to store data in key-value pairs, creating a relationship between a unique identifier (the key) and its associated data (the value). Unlike sequences like lists or tuples, which are indexed by a range of numbers, dictionaries are indexed by keys. These keys must be of an immutable (unchangeable) data type, such as strings, numbers, or tuples. This structure is modeled after a real-world dictionary where you look up a "word" (the key) to find its "definition" (the value). One of the most critical aspects of a dictionary is its efficiency; it uses a process called hashing to look up data, which means that finding a value takes roughly the same amount of time regardless of whether the dictionary has ten items.
Key Properties and Behavior

One of the most defining characteristics of a dictionary is that keys must be unique. As you demonstrated in your Ford example, if you attempt to assign a value to a key that already exists, Python doesn't throw an error; instead, it simply overwrites the old value with the new one. This makes dictionaries "latest-value" biased. Regarding order, it is important to note that while older versions of Python treated dictionaries as unordered, modern Python guarantees that dictionaries maintain the insertion order. This means that when you iterate through a dictionary, the items will appear in the exact order you added them. However, they remain mutable, meaning you can grow, shrink, or modify them in place without creating a new object in memory, which is why your product price update worked so seamlessly.

Beyond simple storage, dictionaries provide powerful built-in methods for data manipulation and "safe" coding. For instance, using student["name"] is direct, but it can be risky; if the key "name" doesn't exist, your program will crash with a KeyError. This is where the .get() method becomes essential, as it allows you to provide a fallback value (like "Student not found") if the key is missing. Furthermore, dictionaries provide "view objects" through methods like .keys(), .values(), and .items(). These aren't just static lists; they are dynamic windows into the dictionary. If you change the dictionary, the view object reflects that change immediately without needing to be refreshed. This linked behavior is what makes dictionaries the go-to tool for complex tasks like user authentication, data counting, and representing real-world objects in your code.
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
