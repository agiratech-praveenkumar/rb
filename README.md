# Ruby 
## Control Statements
----
####  What is control statement? 

A control statement is a statement that determines whether other statements will be executed.

- if
- if - else
- if - elsif
- unless
- terinary
- case statement

these are the types in ruby for making decisions.


### Operators

| Symbol | Meaning |
| :----: | :----: |
| < | Less Than |
| > | Greater than |
| == | Equals |
| != | Not Equals |
| >= | Greater OR equal to |
| <= | Lesser than OR equal to |

### IF Statement: 
----
IF statements are used to execute when the condition is true.

For ex:
```ruby
quantity = 0

if quantity < 1
  puts "Product is out of Stock!"
end
```

### IF - Else Statement
----
IF Else statement will execute else statement if the condition is false.

For Ex:
```ruby
is_admin = true

if is_admin
    "Welcome Admin!"
else
    "You are Not Authorized!"
end
```

### IF - Elsif Statement
----
IF Elsif statement will check if the next IF statement if the first IF statement false.

```ruby
blood_group = "O"

if blood_group == "A"
  "Can give blood to A and AB"
elsif blood_group == "B"
  "Can give blood to B and AB"
elsif blood_group == "AB"
  "Can give blood to AB"
 else
   "Can give blood to A, B, AB and O"
end
```









