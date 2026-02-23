## exercise 2 Strengthening Through Variations
```python
def check_palindrome(text):
    # Step 1: Clean the string
    cleaned = ""
    for char in text:
        if char.isalnum():      # Keep only letters and numbers
            cleaned += char.lower()

    # Step 2: Compare characters from both ends
    left = 0
    right = len(cleaned) - 1

    while left < right:
        if cleaned[left] != cleaned[right]:
            return f"Not a palindrome. Mismatch at position {left} and {right}"
        left += 1
        right -= 1

    return "It is a palindrome!"

```
##     Reflect on what AI added that you didn't consider initially.

the spacing and puntuation
