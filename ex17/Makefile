# When Make starts, it automatically creates Make variables out of all the environment variables that are set when it's executed
#
# Run this with "export shell_env_var='I am an environment variable'; make"
all:
	# Print out the shell variable
	echo $$shell_env_var

	# Print out the Make variable
	echo $(shell_env_var)
