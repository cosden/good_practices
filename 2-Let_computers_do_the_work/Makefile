###########################################################################
# Simple Makefile example
# 
# Does not compile or build code, simply meant to demonstrate the basics 
# of the utility
#
# Usage consistant with GNU Make.  
# Run "make" to run the "all" target
#
#   Ian Cosden
#   icosden@princeton.edu
# #########################################################################



# protect against files named the same as the targets
.PHONY: all hello_world generate_files populate_files clean

# Because this is the first target it is the default and runs all 
# targets listed  
all: hello_world generate_files populate_files


hello_world:
	@echo "Hello World!"

generate_files:
	@echo "Creating empty text files..."
	touch file-{1..5}.txt

populate_files:
	@echo "Adding text to each file..."
	@echo "new_text" | tee -a *.txt > /dev/null

# Not included in all, to be run to delete txt files
# Use "make clean" to run
clean:
	@echo "Cleaning up..."
	rm *.txt
