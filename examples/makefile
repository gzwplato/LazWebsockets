all: bin bin/chatServer bin/chatClient

FPC_OPT=-g -gh -Ci -Cr -Co -Ct -CR -Sa
	
clean:
	rm -rf bin

bin:
	mkdir bin

bin/%: %.pas ../src/*.pas
	fpc -Fu../src -FE./bin ${FPC_OPT} $< ;\
		rm bin/*.o bin/*.ppu
