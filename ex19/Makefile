new_contents = "hello:\n\techo \$$(cooly)"

all:
	mkdir -p subdir
	printf $(new_contents) | sed -e 's/^ //' > subdir/Makefile
	@echo "---MAKEFILE CONTENTS---"
	@cd subdir && cat Makefile
	@echo "---END MAKEFILE CONTENTS---"
	cd subdir && $(MAKE)

# Note that variables and exports are set/affected globally
cooly="The subdirectory can see me!"
export cooly
# This would nullify the line above: unexport cooly

clean:
	rm -f subdir
