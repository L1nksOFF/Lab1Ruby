# Lab1Ruby

Розділ introduction-to-ruby

1. Set the following variables to the corresponding values:

my_num to the value 25
my_boolean to the value true (note the capitalization!)
my_string to the value "Ruby"

my_num = 25     # Add your code here!

my_boolean = true     # And here!

my_string = ("Ruby")     # Also here.

puts my_num
puts my_boolean
puts my_string

2. Set the variable my_num to the value 100, then click the Run button to run your code.

my_num = 100

# Write code above this line!

puts my_num

3. Do a little math practice in the editor. When you’re ready, click Next.

Do a little math practice in the editor. When you’re ready, click Next.

4. In the editor, use at least one print statement and at least one puts statement. You can print out any strings you like! (Make sure to put your strings between quotes, like this: "Hello!".)

puts "Hello World"
print "Hello World"

5. Call the .length method on your name (remember to use quotes around your name).
puts the answer to the console if you want to see the value.

puts "laboratorna1".length

6. Call the .reverse method on your name. Don’t forget those quotation marks around your name to make it a string!
puts the answer to the console if you want to see the value.

puts "Lab1".reverse

7. Call .upcase on your name to make your name ALL CAPS and use puts to print it to the screen, like this:
puts "eric".upcase    # ==> ERIC
On the next line, call .downcase to make your name all lower case. Make sure to use puts so you can see it printed out!

puts "vlad".upcase
puts "vlad".downcase 

8. Write a comment in the editor. It can be anything you like!

puts "vlad".upcase #name

9. Create a multi-line comment in the editor to the right. Make sure =begin and =end are on their own lines!

=begin
Hello everyone!
It's just code...
=end

10. Create a variable name in the editor and set it equal to your name as a string (between quotes, like this: "Eric"). Your string can be capitalized, but name should be all lower case!

name = "Vlad"

11. Create a variable called my_name and set it equal to your name as a string. Create a second variable called my_age and set it equal to your age as a number (don’t use any quotes around the number).

my_name = "Vlad"
my_age = 19;

12. In the editor, set the variables:
sum equal to 13 + 379
product equal to 923 * 15
quotient equal to 13209 / 17
Print each variable to the console using puts if you want to see the results.

sum = 13 + 379
product = 923 * 15
quotient = 13209 / 17

puts sum
puts product
puts quotient

13. Declare a variable name and set it equal to a string containing your name. Call .downcase on your name to make it all lower case, call .reverse on your lowercase name to make it backwards, then call .upcase on your backwards name to make it ALL CAPS.
In Ruby, you can do this two ways: each method call on a separate line, or you can chain them together, like this:
name.method1.method2.method3
puts the method call if you want to see the result.

name = "Vlad"
name = name.downcase
name = name.reverse
name = name.upcase

puts name

14. Create a single-line comment and a multi-line comment in the editor to the right. (Check the Hint if you need a reminder on the syntax.) Hit Run to see your glorious comments and complete the Introduction to Ruby!

# This is a single-line comment

=begin
This is a
multi-line comment
=end



Розділ putting-the-form-in-formatter

1. print the question "What's your first name?" to the screen. Feel free to peek back at the first exercise if you need a syntax reminder.

print "What's your first name?"

2. Declare a variable first_name and set it equal to gets.chomp.
This checkpoint may seem like it’s running forever, but the terminal to the right is actually waiting for input because of gets.chomp. Answer the question in the terminal and press “Enter” or “Return” to finish checking your work.

print "What's your first name?"
first_name = gets.chomp

3. Add print prompts, variables, and gets.chomps for the user’s last name, city, and state/province. Use last_name as the variable for the user’s last name, city for their city, and state for their state or province. (Hint: prompt the user to provide an abbreviation for their state or province, such as “NY” for New York. This will naturally lead us to use .upcase later!)
After pressing Run, type a response in the console and hit enter for each prompt.

print "What's your first name?"
first_name = gets.chomp

print "What's your last name? "
last_name = gets.chomp

print "What city are you from? "
city = gets.chomp

print "What state are you from? "
state = gets.chomp
state.upcase!

4. Let’s use this syntax to print out the values of first_name, last_name, city, and state using #{} syntax.
Press the Run button to test your code. Don’t forget to enter your answers in the console!

print "What's your first name?"
first_name = gets.chomp

print "What's your last name? "
last_name = gets.chomp

print "What city are you from? "
city = gets.chomp

print "What state are you from? "
state = gets.chomp
state.upcase!

puts "Your name is #{first_name} #{last_name} and you are from #{city}, #{state}!"

5. After each variable assignment: first_name, last_name, and city add the .capitalize! method
For state use the .upcase! method
Press Run to test your code. Don’t forget to enter your answers in the console!

print "What's your first name?"
first_name = gets.chomp
first_name.capitalize!

print "What's your last name? "
last_name = gets.chomp
last_name.capitalize!

print "What city are you from? "
city = gets.chomp
city.capitalize!

print "What state are you from? "
state = gets.chomp
state.upcase!

puts "Your name is #{first_name} #{last_name} and you are from #{city}, #{state}!"



Розділ control-flow-in-ruby

1. Check out the code in the editor. There’s some new syntax there, but we’ll bet you can guess what it does. Click Run to see the program in action! (Go ahead and give Ruby an integer—that is, a positive or negative number with no decimal bit.)

print "Integer please: "
user_num = Integer(gets.chomp)

if user_num < 0
  puts "You picked a negative integer!"
elsif user_num > 0
  puts "You picked a positive integer!"
else
  puts "You picked zero!"
end

2. Write your own if statement in the editor. It can take any expression you want (even just true!), but it should evaluate to true. When it does, it should print a string of your choice to the console (using print or puts).

if 2 > 1
  print "WOW"
end

3. Try it yourself in the editor! Use any expression you like in your if/else statement, but make sure both branches print a string of your choice to the console.

if 1>2
    print "WOW"
else
    print "NOT WOW"
end

4. Add an elsif block to your if/else statement in the editor.

if 1>2
    print "WOW"
elsif 2>3
    print "WOW X2"
else
    print "NOT WOW"
end

5. We’ve started you off in the editor. Replace the ___s with the correct unless statement code so your program prints out "I'm writing Ruby programs!"

hungry = false

unless hungry
  puts "I'm writing Ruby programs!"
else
  puts "Time to eat!"
end

6. We’ve got two variables in the editor: is_true and is_false. Replace the __ with == or != to make is_true evaluate to true and is_false evaluate to false.

is_true = 2 != 3

is_false = 2 == 3

7. We’ve set up a few variables in the editor. We want them all to evaluate to true. Your job: replace the __s with <, <=, >, or >= to make the expression for each variable true!

test_1 = 17 > 16

test_2 = 21 < 30

test_3 = 9 <= 9

test_4 = -11 <= 4

8. For this round, we’ll show you the comparators and you set each variable to true or false depending on what value you expect the expression to return. Remember: no quotes around true and false!

# test_1 = 77 != 77
test_1 = false

# test_2 = -4 <= -4
test_2 = true

# test_3 = -44 < -33
test_3 = true

# test_4 = 100 == 1000
test_4 = false

9. Let’s practice a bit with &&. Check out the boolean expressions and set each variable to true or false depending on what value you expect the expression to return.

# boolean_1 = 77 < 78 && 77 < 77
boolean_1 = false

# boolean_2 = true && 100 >= 100
boolean_2 = true

# boolean_3 = 2**3 == 8 && 3**2 == 9
boolean_3 = true

10.Set each variable to true or false depending on what value you expect the expression to return.

# boolean_1 = 2**3 != 3**2 || true
boolean_1 = true

# boolean_2 = false || -10 > -9
boolean_2 = false

# boolean_3 = false || false
boolean_3 = false

11. Set each variable to true or false depending on what value you expect the expression to return.

# boolean_1 = !true
boolean_1 = false

# boolean_2 = !true && !true
boolean_2 = false

# boolean_3 = !(700 / 10 == 70)
boolean_3 = false

12. Last one! Set each variable to true or false depending on what value you expect the expression to return.

# boolean_1 = (3 < 4 || false) && (false || true)
boolean_1 = true

# boolean_2 = !true && (!true || 100 != 5**2)
boolean_2 = false

# boolean_3 = true || !(true || false)
boolean_3 = true

13. Create an if/else statement in the editor. Make sure to include at least one elsif. Each branch of the statement should print something to the console.

a = 10
b = 11
if a < b
  print "a is less than b!"
elsif b < a
  print "b is less than a!"
else
  print "b is equal to a!"
end

14. Create an unless statement in the editor. The statement should print something to the console.

unless false
puts "wow"
end

15. We’re letting you know what value (true or false) we want each variable to have, and your job is to add an expression that evaluates to the correct value using comparators.

# test_1 should be false
test_1 = 5 >= 10

# test_2 = should be false
test_2 = 4 > 5

# test_3 = should be true
test_3 = 2 > 1

16. The code in the editor indicates what value (true or false) we want each variable to have, and your job is to add an expression that evaluates to the correct value using boolean operators (&&, ||, or !).

( 1 == 1 ) && ( 2 == 2 )  # true
( 1 == 2 ) || ( 2 == 2 ) # true
!( false ) # true




Розділ thith-meanth-war

1. Click Run to see the Daffy Duckifier in action and to start building your own!

print "Thtring, pleathe!: "
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
  user_input.gsub!(/s/, "th")
else
  puts "Nothing to do here!"
end
  
puts "Your string is: #{user_input}"

2. Use print to ask the user for input.
Declare a variable called user_input and set it equal to the user’s input using gets.chomp.

print "What is your name?"
user_input = gets.chomp

3. Call the .downcase! method on user_input. Make sure to include the ! so that the user’s string is modified in-place; otherwise, Ruby will create a copy of user_input and modify that instead.

print "What is your name?"
user_input = gets.chomp.downcase!

4. We want to check user_input for the substring "s".

Write an if statement in the editor. It should check to see if user_input includes "s".

For now, print a string of your choice to the console if it finds "s".

After running the code, make sure to enter a string in the terminal.

print "What is your name?"
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
end

5. Remove the print statement you added to your if statement and replace it with a call to .gsub! on user_input. Have it replace /s/ with "th".

After pressing Run, enter a message in the console and hit enter to check your code!

print "What is your name?"
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
user_input.gsub!(/s/, "th")
end

6. Add an else statement that displays a string to the user to let them know if there are no “s”s in their string.

print "What is your name?"
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
user_input.gsub!(/s/, "th")
else
    puts "S not found"
end

7. Add a puts statement that uses string interpolation to show the user their transformed string.

print "What is your name?"
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
user_input.gsub!(/s/, "th")
else
    puts "S not found"
end

8. Enough pondering for now. When you’re ready, click Run to complete this project.

print "What is your name?"
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
user_input.gsub!(/s/, "th")
else
    puts "S not found"
end



Розділ the-while-loop

1. The while loop in the editor is currently an infinite loop. Correct it so it will end! (Be careful—if you click Run right away, you’ll start the infinite loop and you’ll have to refresh the page.)

i = 0
while i < 5
  puts i
  # Add your code here!
    i = i + 1
end

2. On line 2, fill in the __ blank so that the loop breaks when counter is greater than 10.

On line 5, increment counter like we do in the example above.

counter = 1
until counter == 11
  puts counter
  # Add code to update 'counter' here!
    counter += 1
end

3. The loop from the first exercise is in the editor. Rewrite it using the appropriate assignment operator.

counter = 1
while counter < 11
  puts counter
  counter += 1
end

4. Update the for loop in the editor in two ways:

Make it print the numbers 1 to 15, including 15.
Change it to use .. instead of ....

for num in 1..15
  puts num
end

5. Write a for loop that puts the numbers 1 to 20, including 20, using either .. or .... Check Hint if you need a syntax refresher.

for num in 1..20
  puts num
end

6. Replace the ___s in the editor with the appropriate keywords. Check the Hint if you need help!

i = 20
loop do
  i -= 1
  print "#{i}"
  break if i <= 0
end

7. Add a line to your loop before your print statement. Use the next keyword so that you skip to the next iteration if the number i is odd.

Use the example above for help, but remember that the example above skips even numbers.

i = 20
loop do
  i -= 1
  next if i % 2 == 1
  print "#{i}"
  break if i <= 0
end

8. Create a variable called my_array and set it equal to the numbers 1 through 5, inclusive, in order.

my_array = [1, 2, 3, 4, 5]

9. Use the .each method on the odds array to print out double the value of each item of the array. In other words, multiply each item by 2.Make sure to use print rather than puts, so your output appears on one line.

Check the Hint if you get stuck!

odds = [1,3,5,7,9]

# Add your code below!

odds.each do |item|
item *= 2
print item
end

10. Use the .times operator to print out a string of your choice any number of times you like. Use the code in the text above as a guide if you need help.

90.times { print "hi" }

11. Use a while loop to print out the numbers 1 through 50, inclusive. While the example above counts down, you will want to count up.Use print rather than puts, and don’t forget to increment your variable.

i = 1
while i <= 50
  print i
  i += 1
end

12. Now rewrite your while loop using until. You still want to print out the numbers 1 through 50, inclusive.

i = 1
until i == 51
  print i
  i += 1
end

13. Now print out the numbers from 1 to 50 inclusive, using a for loop instead of an until loop.

i = 1
for i in  1..50 
  print i
  i += 1
end

14. Use the loop iterator to print out the string "Ruby!" 30 times.

Make sure to type the string exactly as shown!

i = 0
loop do
  print "Ruby!"
  i += 1
  break if i == 30
end

15. Use the .times iterator to print "Ruby!" to the console 30 times. Hit Run to see the majesty of your code and complete this lesson!

30.times { print "Ruby!" }



Розділ redacted

1. Use puts to prompt the user for input two times. For the first puts, declare a variable called text and set it equal to the user’s input via gets.chomp.

For the second puts, declare a variable called redact and set it equal to the user’s input using gets.chomp.

Note: When running code that includes gets, remember to give input for the terminal. When it expects input but never receives it an error will be displayed after some time. This prevents it from running indefinitely.

puts "Enter text: "
text = gets.chomp

puts "Enter text: "
redact = gets.chomp

2. Declare a variable called words and set it equal to the result of calling the .split method on text. Pass .split a space (" ") to use as a delimiter so that we get an array made up of the words from text.

When running the code, be sure to enter text and words to redact in the console!

puts "Enter text: "
text = gets.chomp

puts "Enter text: "
redact = gets.chomp

words = text.split(" ")

3. Let’s start simple: write an .each loop that iterates through words and just prints out each word it finds.

puts "Enter text: "
text = gets.chomp

puts "Enter text: "
redact = gets.chomp

words = text.split(" ")

words.each do |i|
    print i
end

4. Add an if/else statement inside your .each.

if the current word equals the word to be redacted, then print "REDACTED " with that extra space.
Otherwise (else), print word + " ".
The extra space in both cases prevents the words from running together.

puts "Enter text: "
text = gets.chomp

puts "Enter text: "
redact = gets.chomp

words = text.split(" ")

words.each do |i|
    if i != redact
    print i + " "
else
    print "REDACTED "
  end
end



Розділ ruby-data-structures

1. Declare a variable, my_array, in the editor, and set it equal to an array of your choice. Check the Hint if you need a syntax refresher.

my_array = [1, 3, 5, 7]

2. Use square bracket notation to print the third value of demo_array to the console.

Remember that the third value is at index 2, not at index 3. We start counting indices from zero.

demo_array = [100, 200, 300, 400, 500]

print demo_array[2]  # Add your code here!

3. Create a new array called string_array. Make it an array of… strings!

string_array = ["aaa", "aaa", "aaa"]

4. Create your own two-dimensional array called my_2d_array in the editor. The elements of the inner array(s) can be anything you like: numbers, strings, booleans, and so on. Check the Hint if you need help.

my_2d_array = [[1, 2, 3, 4, 5], ["aaa", "aaa", "aaa"], [true, false]]

5. Use Hash.new to create a new hash called pets. Hash must be capitalized, or Ruby won’t know what you’re talking about!

pets = Hash.new

6. Add a pet to your pets hash. It can be any key-value pair you like!

pets = Hash.new
pets["Murchik"] = "cat"

7. Access the key-value pair you added to pets, just like step 2 in the example above.

Use puts to print that value to the console.

pets = Hash.new
pets["Murchik"] = "cat"
puts pets["Murchik"]

8. Use the .each iterator to puts out each element of the languages array.

Make sure to use puts instead of print, so each element is on its own line.

languages = ["HTML", "CSS", "JavaScript", "Python", "Ruby"]

languages.each { |element| puts element }

9. Puts out every element inside the sub-arrays inside s.

Iterate through .each element in the s array. Call the elements sub_array.
Then iterate through .each sub_array and puts out their items.

s = [["ham", "swiss"], ["turkey", "cheddar"], ["roast beef", "gruyere"]]

s.each { |sub_array| sub_array.each { |element| puts element }}

10. Use .each to iterate over the secret_identities hash.

Use puts to print each key-value pair, separated by a colon and a space (:), to the console, just like the example above.

secret_identities = {
  "The Batman" => "Bruce Wayne",
  "Superman" => "Clark Kent",
  "Wonder Woman" => "Diana Prince",
  "Freakazoid" => "Dexter Douglas"
}
  
secret_identities.each do |nick, name|
  puts "#{nick}: #{name}"
end

11. Create your own multidimensional array called my_array in the editor. The elements of the innermost array can be anything you like: numbers, strings, booleans, and so on. Check the Hint if you need help.

my_array = [[1, 2, 3, 4, 5], ["a", "a", "a"], [false, true]]

12. Create a hash called my_hash in the editor.

Give it at least one key-value pair.

my_hash = { 
  "a" => 1,
}

13. Iterate through .each key/value pair in lunch_order.

Please puts out the value of each pair (just the value, not the key).

lunch_order = {
  "Ryan" => "wonton soup",
  "Eric" => "hamburger",
  "Jimmy" => "sandwich",
  "Sasha" => "salad",
  "Cole" => "taco"
}

lunch_order.each { |name, nfood| puts nfood }



Розділ create-a-histogram

1. Use a puts statement to prompt the user for input. Use gets.chomp to save this input to a variable called text.

puts "Text please: "
text = gets.chomp

2. Declare a variable called words and set it equal to the result of calling .split on text.

puts "Text please: "
text = gets.chomp
words = text.split(" ")

3. Create a hash called frequencies in the editor.

Give it a default value of 0.

After pressing Run, enter a message in the console and hit enter to check your code!

puts "Text please: "
text = gets.chomp
words = text.split(" ")
frequencies = Hash.new(0)

4. Use .each to iterate over the words array.

For each word we find, assume that the word itself is a key in frequencies and increment its value by 1.

This is why our default is 0. The first time we find the word, it will have a default value of 0 that we can increment by 1.

Take a look at the Hint if you need help.

puts "Text please: "
text = gets.chomp
words = text.split(" ")
frequencies = Hash.new(0)
words.each { |word| frequencies[word] += 1 }

5. Use .sort_by to sort the frequencies hash by word count, like step 2 above. Store the result back in frequencies.

Use .reverse! to reverse the sorted frequencies array.

Check the Hint for more details!

puts "Text please: "
text = gets.chomp
words = text.split(" ")
frequencies = Hash.new(0)
words.each { |word| frequencies[word] += 1 }
frequencies = frequencies.sort_by {|a, b| b }

6. Iterate over .each key/value pair in the frequencies hash.

Then, puts each word, a single space, and its frequency to the console, like in the example above.

puts "Text please: "
text = gets.chomp
words = text.split(" ")
frequencies = Hash.new(0)
words.each { |word| frequencies[word] += 1 }

frequencies = frequencies.sort_by do |word, count|
  count
end

frequencies.reverse!

frequencies.each do |word, count|
  puts word + " " + count.to_s
end



Розділ methods-blocks-sorting

1. We’ve started a method in the editor to the right, but it’s incomplete. Replace the ___s with the correct keywords so the method will work!

def puts_1_to_10
  (1..10).each { |i| puts i }
end

puts_1_to_10 # Ignore this for now. We'll explain it soon!

2. Create a method, greeting, in the editor. It should use puts to print a greeting to the console.

# Define your method below!

def greeting
# Define your method above this line.
  puts "greeting"
end

greeting # Ignore this for now. We'll explain
         # it in the next exercise!
         
3. We’ve set up a function, array_of_10, in the editor to the right. Call it on line 5!

def array_of_10
  puts (1..10).to_a
end

4. Call the cubertino method in the editor, passing it an argument of 8.

def cubertino(n)
  puts n ** 3
end

cubertino(8)

5. Define a new method called add that takes two numbers as parameters.
Inside the method, return the sum of those numbers.

def add(x, y)
  return x + y
end

6. Define a method called greeter that takes a single string parameter, name, and returns a string containing that person’s name.
Make sure to return the string. Don’t use print or puts.

Define a by_three? method that takes a single integer parameter, number, and returns true if that number is evenly divisible by three and false if not.

def greeter(name)
  return "Hey, #{name}!"
end

def by_three?(number)
  if number % 3 == 0
    return true
  else
    return false
  end
end

7. Currently, the second .each will print out 5 five times (since it will print 5 for each item in the array, and there are five items). Modify the block so it will print each item in the array multiplied by five.

# The block, {|i| puts i}, is passed the current
# array item each time it is evaluated. This block
# prints the item. 
[1, 2, 3, 4, 5].each { |i| puts i }

# This block prints the number 5 for each item.
# (It chooses to ignore the passed item, which is allowed.)
[1, 2, 3, 4, 5].each { |i| puts 5*i }

8. Use the .sort! method to sort the values in my_array. Magic, isn’t it?

Display my_array in the console.

my_array = [3, 4, 8, 7, 1, 6, 5, 9, 2]

# Call the sort! method on my_array below.
# my_array should then equal [1, 2, 3, 4, 5, 6, 7, 8, 9].

my_array.sort!
puts my_array

9. What Ruby method could we call on books in order to sort the list of books alphabetically? Try it out in the editor.

# library sorting code
books = ["Charlie and the Chocolate Factory", "War and Peace", "Utopia", "A Brief History of Time", "A Wrinkle in Time"]

# How might we sort! the books in alphabetical order? (Hint, hint)

books.sort!
puts books

10. Use the combined comparison operator to compare book_1 to book_2 (in that order). Before you run the code, think about what the result will be.

book_1 = "BOOK1"

book_2 = "BOOK2"

book_1 <=> book_2

11. Sort your books in descending order on line 8. Use the example of sorting in ascending order on line 4 as a guide.

Display the result in the console.

books = ["Charlie and the Chocolate Factory", "War and Peace", "Utopia", "A Brief History of Time", "A Wrinkle in Time"]

# To sort our books in ascending order, in-place
books.sort! { |firstBook, secondBook| firstBook <=> secondBook }

# Sort your books in descending order, in-place below

books.sort! { |firstBook, secondBook| secondBook <=> firstBook }

12. Create a method, welcome, that puts “Welcome to Ruby!” After defining your method, call it.

def welcome
  puts "Welcome to Ruby!"
end

welcome

13.Change your welcome method definition. Add a single string parameter called name.

Remove your puts statement and replace it with return "Hello, #{name}"

def welcome(name)
  return "Hello, #{name}!"
end

welcome("NAME")

14. def welcome(name)
  return "Hello, #{name}!"
end

welcome("NAME")

15. Add a block after .each that multiplies each item by itself and puts the result to the console.

my_array = [1, 2, 3, 4, 5]

my_array.each do |num|
  puts num * num
end

16. Use .sort! to sort the fruits array in descending (that is, reverse) alphabetical order. You can use the combined comparison operator (like the example above) or an if/elsif/else statement.

fruits = ["orange", "apple", "banana", "pear", "grapes"]

fruits.sort! do |fruitOne, fruitTwo| 
  fruitTwo <=> fruitOne
end



Розділ ordering-your-library

1. The code in the editor should look familiar—there’s only one new idea (on line 1). When you’re ready, click Run to execute the code and start building your own method.

def alphabetize(arr, rev=false)
  if rev
    arr.sort { |item1, item2| item2 <=> item1 }
  else
    arr.sort { |item1, item2| item1 <=> item2 }
  end
end

books = ["Heart of Darkness", "Code Complete", "The Lorax", "The Prophet", "Absalom, Absalom!"]

puts "A-Z: #{alphabetize(books)}"
puts "Z-A: #{alphabetize(books, true)}"

2. Define alphabetize in the editor to the right. It shouldn’t take any arguments yet, and there doesn’t need to be anything in the body of the method.

def alphabetize
end

3. Update your alphabetize method with two parameters: arr, representing the array to be passed in, and rev, a boolean that defaults to false.

def alphabetize(arr, rev = false)
end

4. Inside your method, add a line that calls .sort! on the arr array. Since it is the last line of the method, the sorted array will be returned.

Now test your work! After your method, make a new array called numbers that contains a few numbers like the example above.

Call your alphabetize method with your numbers array as the parameter and puts the result to the console.

def alphabetize(arr, rev = false)
  arr.sort!
end

numbers = [3, 5, 1, 6]

puts alphabetize(numbers)

5. After your .sort! call, add an if-else statement. If rev is true, call reverse! on arr, else return arr.

Keep your numbers array and the puts statement so that you can see your work in action!

def alphabetize(arr, rev = false)
  arr.sort!
  if rev == true
    arr.reverse!
  else
  	arr
  end
end

numbers = [3, 5, 1, 6]

puts alphabetize(numbers)



Розділ hashes-and-symbols

1. Create a hash called my_hash using whichever method you prefer.

my_hash = { "a" => 1,
  					"b" => 2
}

2. Iterate over the matz hash and print each value to the console using puts.

matz = { "First name" => "Yukihiro",
  "Last name" => "Matsumoto",
  "Age" => 47,
  "Nationality" => "Japanese",
  "Nickname" => "Matz"
}

matz.each do |key, value|
  puts value
end

3. Go ahead and try to access a key in creatures that doesn’t exist.

creatures = { "weasels" => 0,
  "puppies" => 6,
  "platypuses" => 3,
  "canaries" => 1,
  "Heffalumps" => 7,
  "Tiggers" => 1
}

creatures["birds"]

4. In the meantime, create a hash called no_nil_hash and give it any default value other than nil.

no_nil_hash = Hash.new("Never nil!")

5. All right! Time to create your first symbol. Create a regular old variable called my_first_symbol and set it equal to any valid symbol you like!

# Write your code below!

my_first_symbol = :my_symbol

6. Add at least two more keys to the symbol_hash hash replacing the ______ blanks.

The keys should all be symbols; their associated values can be anything you like.

symbol_hash = {
  :one => 1,
  :two => 2,    # Fill in these two blanks!
  :three => 3,
}

7. We have an array of strings we’d like to later use as hash keys, but we’d rather they be symbols.

Create a new variable, symbols, and store an empty array in it.
Use .each to iterate over the strings array.
For each s in strings, use .to_sym to convert s to a symbol and use .push to add that new symbol to symbols.
Print the symbols array.
Check the hint for a more information on how to use .each and .push.

strings = ["HTML", "CSS", "JavaScript", "Python", "Ruby"]
symbols = []

strings.each do |s| 
 symbols.push(s.to_sym)
end 
print symbols

8. Update your code from the last exercise to use .intern instead of .to_sym.

strings = ["HTML", "CSS", "JavaScript", "Python", "Ruby"]
symbols = []

strings.each do |s| 
 symbols.push(s.intern)
end 
print symbols

9. Create a hash called movies with symbols as keys and strings as values.

Inside your hash, add two key/value pairs.

The keys should be the names of movies.

The values should be quick descriptions or reviews.

Check out the Hint if you want an example to get you started!

movies = {
  :children => "Moana",
  :scifi => "Mortal Kombat",
  :history => "Lincoln"
}

10. Create a hash called movies with symbols as keys and strings as values.

Inside your hash, add two key/value pairs.

The keys should be the names of movies.

The values should be quick descriptions or reviews.

Check out the Hint if you want an example to get you started!

movies = {
  :children => "Moana",
  :scifi => "Mortal Kombat",
  :history => "Lincoln"
}

11. Update your hash from the previous exercise to use the new 1.9 hash syntax instead of the older hash rocket syntax.

movies = {
  children: "Moana",
  scifi: "Mortal Kombat",
  history: "Lincoln"
}

12. Create a new variable, good_movies, and set it equal to the result of calling .select on movie_ratings, selecting only movies with a rating strictly greater than 3.

movie_ratings = {
  memento: 3,
  primer: 3.5,
  the_matrix: 5,
  truman_show: 4,
  red_dawn: 1.5,
  skyfall: 4,
  alex_cross: 2,
  uhf: 1,
  lion_king: 3.5
}

good_movies = movie_ratings.select { |name, rating| rating > 3 }

13. Go ahead and print out just the titles of our movies using puts.

movie_ratings = {
  memento: 3,
  primer: 3.5,
  the_matrix: 3,
  truman_show: 4,
  red_dawn: 1.5,
  skyfall: 4,
  alex_cross: 2,
  uhf: 1,
  lion_king: 3.5
}
# Add your code below!

movie_ratings.each_key { |title| puts title }
