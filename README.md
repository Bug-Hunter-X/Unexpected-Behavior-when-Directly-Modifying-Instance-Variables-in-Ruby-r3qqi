# Ruby Instance Variable Modification Bug

This example demonstrates a potential issue when directly manipulating instance variables in Ruby using `instance_variable_set`. While functional, this practice can make code less maintainable and lead to unexpected behavior if you've implemented getter/setter methods with specific logic.

## Bug
The `bug.rb` file showcases how modifying the `@value` instance variable directly bypasses any custom getter/setter methods that might be in place, potentially causing errors or inconsistencies.

## Solution
The `bugSolution.rb` illustrates the improved approach where instance variables are accessed and modified through methods, ensuring adherence to any defined logic and maintaining better code structure and maintainability.