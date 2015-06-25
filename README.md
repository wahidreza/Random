# Random
#experiment 5, raw_input and printing
#26.06.2015

# Questions: 
my_name = raw_input("What is your name? ")
my_age = raw_input("How old are you? ")
print "type 'nothing' if you DON'T have a hobby"
hobby = raw_input("What is your hobby? ") 
if hobby == "nothing":
	hobby = "I don't have a hobby"
else:
	hobby = "I have %s as a hobby" % hobby
kglbs = raw_input("Will you enter your weight in kg or lb? ")
my_weight = int(input("What is your weight? "))
if kglbs == "kg":
		my_weight = "%s kg" % my_weight
if kglbs == "lb":
		my_weight = "%s lb" % my_weight

ht = raw_input("Will you enter your height in inches or cm? ")

if ht == "cm":
		my_height = raw_input("What is your height? ")
if ht == "inches":
		my_heightft = int(input("How many feet? "))
		my_heightinches = int(input("How many inches? "))
		q_con = raw_input("Do you wish to convert your height into cm? Yes or no? ")
		if q_con == "yes":
			my_height = my_heightft * 30.48 + 2.54 * my_heightinches
			my_height = "%d cm" % my_height
		#my_height = "%d ft and %d inches" % (my_heightft, my_heightinches)

my_eyes = raw_input("What is the color of your eyes? ")
my_hair = raw_input("What is the color of your hair? ")



#kg to lb and vice versa conversion

#if kglbs == "kg":
#	my_weight = my_weight * 2.2046
	
#if kglbs == "lb":
#	my_weight = my_weight / 2.2046

print "Hey, here's some quick things about me!"
print "My name is %s . I am %s years old and %s . I weigh %s and am %s tall. Also, my eyes are %s and I have %s hair." % (my_name, my_age, hobby, my_weight, my_height, my_eyes, my_hair)
