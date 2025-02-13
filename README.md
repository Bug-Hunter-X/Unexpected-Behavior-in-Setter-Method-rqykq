# Unexpected Behavior in Ruby Setter Method

This repository demonstrates an uncommon bug in Ruby related to setter methods and instance variables. The issue arises when directly assigning a value to a method that's also a setter method, without properly updating the instance variable within the setter method. The code produces unexpected results because the direct assignment doesn't affect the instance variable.

## Bug Description
The `value=` method does not correctly update the instance variable `@value` when assigning using the method in the form of `object.value = new_value`. This leads to inconsistent values.