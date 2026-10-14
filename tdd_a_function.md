# {{PROBLEM}} Function Design Recipe


## 1. Describe the Problem

A function called count_words that takes a string as an argument and returns the number of words in that string.

## 2. Design the Function Signature

_Include the name of the function, its parameters, return value_

```python
# EXAMPLE
# function - a function runs when it's called. It's also reusable.

# def function_name(parameters/arguments/input):
    # return output

def count_words(string):
    """Extracts uppercase words from a string

    Parameters/Input: string

    Returns/Output: "number of words in the string" // number/integer

    pass # 
```

## 3. Create Examples as Tests

_Make a list of examples of what the function will take and return._

```python
# EXAMPLE


"""
When the string is empty, return 0
"""
count_words("") => 0

"""
When the string only contains one word, return 1
"""
count_words("abcdefg") => 1

"""
When the string only contains five words, return 5
"""
count_words("This is a sentence yay")


## 4. Implement the Behaviour

_After each test you write, follow the test-driving process of red, green, refactor to implement the behaviour._

Here's an example for you to start with:

```python
# EXAMPLE

from lib.extract_uppercase import *

"""
Given a lower and an uppercase word
It returns a list with the uppercase word
"""
def test_extract_uppercase_with_upper_then_lower():
    result = extract_uppercase("hello WORLD")
    assert result == ["WORLD"]
```

Ensure all test function names are unique, otherwise pytest will ignore them!
