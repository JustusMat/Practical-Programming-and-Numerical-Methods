SPATH = ./source/
BPATH = ./build/
DPATH = ./data/
OPATH = ./output/
APATH = ./animation/

default:
	cd $(BPATH) && $(MAKE)
	cd $(DPATH) && $(MAKE)
	cd $(OPATH) && $(MAKE)
	cd $(APATH) && $(MAKE)

.PHONY: build test

build:
	cd $(BPATH) && $(MAKE)
	
test:
	cd $(BPATH); mono main.exe > ../test.txt

clean:
	$(RM) -rf $(addprefix $(BPATH), *.exe *.dll) 
	$(RM) -rf $(addprefix $(DPATH), *.data) 
	$(RM) -rf $(addprefix $(OPATH), *.txt *.svg *.log) 
	$(RM) -rf $(addprefix $(APATH), *gif)
	$(RM) -rf *.txt 
	clear
	@echo all build, data and output files cleared...