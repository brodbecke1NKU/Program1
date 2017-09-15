# Program1
#!/usr/bin/ruby

# Program 1
# Evan Brodbeck
# CIT 383, 003, Fall 2017
# 9/12/17 

Hash h = Hash.new()
resp = 'y'

while (resp == 'y' or resp == "yes")

    a = Array.new(5)

    puts "Enter your Employee Id"
    employee_id = gets.chomp

    puts "Enter your full name" #ask for full name
    a[0] = gets.chomp #store full name


    puts "Enter Department number"
    department_number = gets
    a[1] = gets.chomp

    puts "Enter the name of your supervisor"
    supervisor = gets
    a[2] = gets.chomp

    puts "Enter your username"
    username = gets
    a[3] = username.chomp

    puts "Enter your password"
    password = gets
    a[4] = password.chomp     
          
    h[employee_id] = a
          
         
    puts "Do you want to add another record?"
    resp = gets.chomp
             
    h.each do |k,v|
        temp = puts k + ' : ' + v.to_s
        put temp
   end 
    
    
    
end 
    
