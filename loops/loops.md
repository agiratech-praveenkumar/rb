# Loops

Looping in programming languages is a feature which clears the way for the execution of a set of instructions or functions repeatedly when some of the condition evaluates to true or false.

Type of Loops
- for
- while 
- do while
- until
- upto and times
- each


### For loop
---

The for loop consists of ```for``` followed by a variable to contain the iteration argument followed by ```in``` and the value to iterate.


```ruby

numbers = Array(0..10)

for i in numbers
	p i
end

```

similarly,

```ruby

fruits = ['apple', 'banana', 'grape', 'orange']

for fruit in fruits
	p fruit
end

```

### While loop
---

The condition which is to be tested, given at the beginning of the loop and all statements are executed until the given boolean condition satisfies.

```ruby

login_attempts = 3

while login_attempts > 0
	p "Remaining Chances #{login_attempts}."
	login_attempts -= 1
end

```

### Do While loop
---

do while loop is similar to while loop with the only difference that it checks the condition after executing the statements.

```ruby

number = 1

loop do
	p "Current number is #{number}"
	number += 1

	break if number > 10
end

```

### Unitl loop
---

The until loop executes while a condition is false.

```ruby

choclate = 0

until choclate > 10
	p "we have #{choclate} choclates."
	choclate += 1
end

```

### Upto and Times
---
Upto and Times are like ranges in ruby.

```ruby
1.upto (10) do |i|
	p i
end
```

similarly,

```ruby
10.times { |i| p i }
```

### Each loop
---

The Ruby method each allows you to go over a list of items, without having to keep track of the number of iterations, or having to increase some kind of counter.


```ruby

numbers = (0..10).to_a

numbers.each { |t| p t**2 }

```

We can also iterate Each with Hash

```ruby
products = {
	dell: 100,
	rog: 200,
	alienware: 400,
	legion: 230,
	mac: 999
}

products.each do |key, value|
	p "Product #{key} is $#{value} dollars."
end
```


## Control Flow Alteration
---
Ruby programming language provides some statements in addition to loops, conditionals, and iterators, which are used to change the flow of control in a program.

- break statement
- next statement
- redo statement
- retry statement
- return statement
- throw/catch statement

&nbsp;   
### break

Break statement is used to exit a loop when the condition is true.

```ruby
x = 2

while true
	p x
	x += 1
	break if x > 22
end
```

### next
next statement is used to jump to the next iterator of given loop.


```ruby
num = (1..10).to_a

for i in num
	next if i.even?
	p i
end
```

### redo
The redo statement is used to restart the current iteration of a loop or the iterator.

```ruby
val = 0
  
while(val < 4)  
	p val
	val += 1
	redo if val == 4
end
```

### retry 

retry statement is used to restart an iterator based on a certain condition.


```ruby
var = 7
  
var.times do |val| 
	p val 
	if val == 6
		var = var - 1 
		retry 
	end  
end

```


### return
This is used to exit from a method, with or without a value.

```ruby
def greet(person="Default Person")
	return "Hello #{person}"
	p "This wont return"
end

greet "Pk"
```

### throw/catch

throw and catch are used to define a control structure which can be considered as a multilevel break. throw is used to break the current loop and transfer the control outside of the catch block. The best thing about throw is that it can break out of the current loop or methods or we can say it can cross any number of levels.

```ruby
def lessNumber(num)
		throw :numberError if num < 10  
    puts "Number is Greater than 10!"
end
  
  
catch :numberError do
    lessNumber(11)
    lessNumber(78) 
      
	# exits catch block here
    lessNumber(7)
    lessNumber(4)
end
  
puts "Outside Catch Block"

```