#cista pro Linux

#balicky, obsahuji doxygen, ale ten se mozna muze samostatne instalovat v doc ?
PACKAGES := $(shell cat requirementsLinux)

#finta
PROJECT = ../PYproj

# idk all je sus, python moc preklad jako nejde nebo jsem stoopid
all: requirementsPython requirementsLinux
	echo "(přeloží projekt)"
	pip3 install -r requirementsPython
	sudo apt-get install $(PACKAGES)

#GITHUB test
#zatim to zipne celej projekt, zpatky do te same slozky
pack: 
	echo "(zabalí projekt tak, aby mohl být odevzdán)"
	zip ZevixCal $(PROJECT) 

#tady asi se bude cleanovat jeste build napr.
clean:
	echo "(smaže všechny soubory, co nemají být odevzdány)"
	rm -rf project/__pycache__

#az nejake budou tak pretty self explenatory
test:
	echo "(spustí testy matematické knihovny)"

#doxygen
doc:
	echo "(spustí generování dokumentace)"

#zapne kalkulacku
run:
	echo "(spustí program)"
	python3 project/test1.py

#tahle sranda jde mimo mne zatim
profile:
	echo "(spustí překlad programu pro výpočet směrodatné odchylky na profiling)"
