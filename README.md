# Grocery-List-Manager-
Description:  Stores grocery items with prices. Calculates total cost Uses dictionary, list, loop, functions, thread, lambda, append, list comprehension, and operators — all very simply.

code:
import threading
# to use thread
# Step 1: Create a dictionary of items and their prices
grocery = {
"apple": 2,
"banana": 1,
"milk": 3
}
# Step 2: Function to calculate total cost
def calculate
_
total():
print("Calculating total...
")
total = 0
for item, price in grocery.items(): # loop through dictionary
total += price # using operator +
print("Total Cost:"
, total)
# Step 3: Run total calculation in a thread
t = threading.Thread(target=calculate
_
total)
t.start()
t.join()
# Step 4: Add a new item using append and list
new
_
items = []
new
_
items.append(("bread"
, 2)) # add tuple to list
new
_
items.append(("eggs"
, 4))
# Step 5: Add new items to dictionary using loop
for name, price in new
items:
_
grocery[name] = price # add to dictionary
# Step 6: Use list comprehension to get all item names
item
_
names = [item for item in grocery]
print("Items:"
, item
_
names)
sorted
# Step 7: Use lambda to sort items by price
_
items = sorted(grocery.items(), key=lambda x: x[1])
print("Sorted by Price:"
, sorted
_
items
