# PyStack

A simple stack implementation in Python.

## Quick start

```python
stack = Stack()  # Create an empty stack.
print(f"This is an empty stack: {repr(stack)}")
stack.push(1)  # Push an item to the stack.
stack.push(2)
stack.push("STR")
print(f"This is a stack with 3 items: {repr(stack)}")  # Show the stack.
print(f"Pop the top item: {repr(stack.pop())}")  # Pop the top item.
print(f"This is a stack with 2 items: {repr(stack)}")
print(f"Pop all items: {repr(stack.pop_all())}")  # Pop all items.
print(f"This is an empty stack: {repr(stack)}")
stack.push_all([4, 5, 6])  # Push all items.
print(f"Now the stack has 3 items: {repr(stack)}")
print(f"The size of the stack is {len(stack)}")  # Get the length of the stack.

del stack[0]  # Delete the first item.
print(f"Delete the first item: {repr(stack)}")

stack_copy = stack.copy()  # Copy the stack.
print(
    f"This is the copy of the stack: {repr(stack_copy)}, {id(stack)} => {id(stack_copy)}"
)
print(f"{stack_copy} == {stack}: {stack_copy == stack}")
```
