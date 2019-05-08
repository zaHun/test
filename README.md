```python

items = ("apple", "mellon")
one, two = items
one, two = two, one
print(one)
# result "mellon"
print(two)
# result "apple"
```
