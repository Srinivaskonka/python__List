"""
Python Lists – All in One Tutorial Code
Author: Konka Srinivas
"""

# 1. Creating lists
```print("\n--- Creating Lists ---")
empty_list = []
fruits = ["apple", "banana", "cherry"]
numbers = list((1, 2, 3, 4))  # Using list() constructor
nested = [[1, 2], [3, 4], [5, 6]]
print(empty_list)
print(fruits)
print(numbers)
print(nested)
```
# 2. Accessing elements
```print("\n--- Accessing Elements ---")
print(f"First fruit: {fruits[0]}")
print(f"Last fruit: {fruits[-1]}")
print(f"Slice [1:3]: {fruits[1:3]}")
```
# 3. Modifying lists
```print("\n--- Modifying Lists ---")
fruits[1] = "blueberry"     # Replace
fruits.append("date")       # Add at end
fruits.insert(1, "banana")  # Insert at position
print(fruits)
```

# 4. Removing elements
```print("\n--- Removing Elements ---")
fruits.remove("banana")  # First match
removed_item = fruits.pop(2)  # Remove by index
print(f"Removed: {removed_item}")
del fruits[0]  # Delete by index
print(fruits)
```

# 5. Common list methods
```print("\n--- List Methods ---")
lst = [3, 1, 4, 1, 5]
print(f"Count of 1: {lst.count(1)}")
print(f"Index of 5: {lst.index(5)}")
lst.sort()
print(f"Sorted: {lst}")
lst.reverse()
print(f"Reversed: {lst}")
copied_list = lst.copy()
print(f"Copied: {copied_list}")
```
# 6. Looping
```print("\n--- Looping Through Lists ---")
for fruit in fruits:
    print(fruit)
for idx, fruit in enumerate(fruits):
    print(f"{idx}: {fruit}")
```
# 7. List comprehensions
```print("\n--- List Comprehensions ---")
squares = [x**2 for x in range(5)]
evens = [x for x in range(10) if x % 2 == 0]
print(f"Squares: {squares}")
print(f"Evens: {evens}")
```
# 8. Nested lists & flattening
```print("\n--- Nested Lists ---")
matrix = [[1, 2], [3, 4], [5, 6]]
print(f"Element [1][0]: {matrix[1][0]}")
flat = [num for row in matrix for num in row]
print(f"Flattened: {flat}")
```
# 9. Copying pitfalls
```print("\n--- Copying Pitfall ---")
list1 = [1, 2, 3]
list2 = list1  # Same reference
list3 = list1.copy()  # New list
list1.append(4)
print(f"list1: {list1}")
print(f"list2 (same ref): {list2}")
print(f"list3 (independent): {list3}")
```
# 10. Sorting with key
```print("\n--- Sorting with Key ---")
words = ["banana", "apple", "cherry"]
words.sort(key=len)  # Sort by length
print(f"Sorted by length: {words}")
```
# 11. Quick cheatsheet in action
```print("\n--- Cheatsheet ---")
lst = [1, 2, 3]
print(lst[0], lst[-1], lst[1:3])  # Access
lst[1] = 99
lst.append(4)
lst.insert(1, 100)
print(lst)
lst.remove(99)
lst.pop()
del lst[0]
print(lst)
lst.clear()
print(f"After clear: {lst}")
```
