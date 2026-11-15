# the export directive takes a variable and sets it the environment for all shell commands in all recipes

shell_env_var = Shell env var, created inside of Make
export shell_env_var
all:
	echo $(shell_env_var)
	echo $$shell_env_var
