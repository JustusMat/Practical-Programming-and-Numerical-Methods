SPATH = ./source/
BPATH = ./build/
DPATH = ./data/
OPATH = ./output/

default:
	cd $(BPATH) && $(MAKE)
	cd $(DPATH) && $(MAKE)		
	cd $(OPATH) && $(MAKE)


.PHONY: build
build:
	cd $(BPATH) && $(MAKE)

clean:
	$(RM) -rf $(addprefix $(BPATH), *.exe *.dll)
	$(RM) -rf $(addprefix $(DPATH), *.data)
	$(RM) -rf $(addprefix $(OPATH), *.txt *.svg *.log)
	clear
	@echo all build and output files cleared 	