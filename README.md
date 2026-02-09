# practical5
Aim : Study Of Python Dictionaries

Theory : 
A Python dictionary is a built-in mapping type that allows you to store data in key-value pairs, creating a relationship between a unique identifier (the key) and its associated data (the value). Unlike sequences like lists or tuples, which are indexed by a range of numbers, dictionaries are indexed by keys. These keys must be of an immutable (unchangeable) data type, such as strings, numbers, or tuples. This structure is modeled after a real-world dictionary where you look up a "word" (the key) to find its "definition" (the value). One of the most critical aspects of a dictionary is its efficiency; it uses a process called hashing to look up data, which means that finding a value takes roughly the same amount of time regardless of whether the dictionary has ten items.
Key Properties and Behavior

One of the most defining characteristics of a dictionary is that keys must be unique. As you demonstrated in your Ford example, if you attempt to assign a value to a key that already exists, Python doesn't throw an error; instead, it simply overwrites the old value with the new one. This makes dictionaries "latest-value" biased. Regarding order, it is important to note that while older versions of Python treated dictionaries as unordered, modern Python guarantees that dictionaries maintain the insertion order. This means that when you iterate through a dictionary, the items will appear in the exact order you added them. However, they remain mutable, meaning you can grow, shrink, or modify them in place without creating a new object in memory, which is why your product price update worked so seamlessly.

Beyond simple storage, dictionaries provide powerful built-in methods for data manipulation and "safe" coding. For instance, using student["name"] is direct, but it can be risky; if the key "name" doesn't exist, your program will crash with a KeyError. This is where the .get() method becomes essential, as it allows you to provide a fallback value (like "Student not found") if the key is missing. Furthermore, dictionaries provide "view objects" through methods like .keys(), .values(), and .items(). These aren't just static lists; they are dynamic windows into the dictionary. If you change the dictionary, the view object reflects that change immediately without needing to be refreshed. This linked behavior is what makes dictionaries the go-to tool for complex tasks like user authentication, data counting, and representing real-world objects in your code.

Algorithm:

A: Update Product Price
1)Start
2)Initialize the dictionary "product" with names as keys and prices as values.
3)Display the "product" dictionary to show the "Original price".
4)Update the value of a specific key using the syntax product["Book"] = "55 Rupees".
5)Display the updated product dictionary.
6)End

B: Search Student Marks
1)Start
2)Initialize the dictionary "student" with names and marks.
3)Input a string from the user and store it in the variable name.
4)Search for the name in the "student" dictionary using the student.get(name,"Student not found" command.
5)Output the mark if the name exists; otherwise, return the default message "Student not found".
6)End

C:User Login Validation
1)Start
2)Initialize the dictionary "users" with usernames as keys and passwords as values.
3)Input data from the user for variables username and password.
4)Validate by checking if users.get(username) matches the entered password.
5)If they match, Display "Login successful".
   Else, Display "Invalid username or password".
6)End  

D:Find Highest Scorer
1)Start
2)Initialize the dictionary "student" with student names and their respective marks.
3)Identify the key with the highest value using max(student, key=student.get) and store it in the variable topper.
4)Access the score of the topper using the syntax student[topper].
5)Display the name of the topper and their corresponding marks.
6)End

Conclusion: 
Hence dictionary was implemented in python and operations were done on them.
