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
