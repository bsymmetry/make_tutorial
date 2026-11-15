#Spaces at the end of a line are not stripped, but those at the start are.  To make a variable with a single space, use $(nullstring)
with_spaces = hello      # with_spaces has many spaces after "hello"
after = $(with_spaces) there

nullstring = 
space = $(nullstring) # Make a variable with a single space

# Use += to append
foo := start
foo += more

all:
	echo "$(after)"
	echo start"$(space)"end

	# an underfined variable is actually an empty string
	echo $(nowhere)

	echo $(foo)
