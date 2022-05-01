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



### Ternary Statement
----

A ternary gives you a way to write a compact if/else expression in just one line of code.

```ruby
rails_version = 6

rails_version == 7 ? "latest version" : "not a latest version"
```
is the same as IF Expression.

```ruby
rails_version = 6

if rails_version == 7
  "latest version"
else
  "not a latest version"
end
```
### Unless Statement
----
The unless expression is the opposite of the if expression. If the value is false, the “then” expression is executed

```ruby
is_user_verified = false

unless is_user_verified
  "User need to be Verified before login."
end
```

We can use else part in unless statement, it works as if statement but inverted.

```ruby
unless is_user_verified
  "User need to be Verified before login."
else
  "Verified User. Login success."
end
```

### Modifier if and unless 

if and unless can also be used to modify an expression. When used as a modifier the left-hand side is the “then” expression and the right-hand side is the “test” expression

#### IF
```ruby
puts "Hello" if true
```
#### Unless
```ruby
puts "World" unless false
```










