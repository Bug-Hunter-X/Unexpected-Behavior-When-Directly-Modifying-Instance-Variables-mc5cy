# Ruby Bug: Unexpected Behavior When Directly Modifying Instance Variables

This repository demonstrates a common Ruby bug related to directly manipulating instance variables using `instance_variable_set` and `instance_variable_get` instead of using accessor methods (getter and setter methods).

**Problem:**
Directly accessing and modifying instance variables bypasses any logic or validation that might be included in getter and setter methods. This can lead to unexpected behavior and make the code harder to maintain and debug.

**Solution:**
Always use accessor methods to interact with instance variables. This ensures data integrity, allows for future modification and extension without breaking the code, and improves the overall readability and maintainability of your code.

**Files:**
- `bug.rb`: Demonstrates the buggy code.
- `bugSolution.rb`: Shows the corrected code using accessor methods.