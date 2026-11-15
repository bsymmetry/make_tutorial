# .EXPORT_ALL_VARIABLES exports all variables for you
#
.EXPORT_ALL_VARIABLES:
new_contents = "hello:\n\techo \$$(cooly)"

cooly = "The subdirectory can see me!"

all:
	mkdir -p subdir
	printf $(new_contents) | sed -e 's/^ //' > subdir/Makefile
	@echo "---MAKEFILE CONTENTS---"
	@cd subdir && cat Makefile
	@echo "---END MAKEFILE CONTENTS---"
	cd subdir && $(MAKE)

clean:
	rm -rf subdir
