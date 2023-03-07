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

