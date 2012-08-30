GHC = ghc 
FLAG = --make -v

SRCNAME=interactWith.hs
SRC=./src/$(SRCNAME)
OBJ=./bin/$(SRCNAME:.hs=.o)

OBJDIR=./obj
HIDIR=./hi

BIN =./bin/$(SRCNAME:.hs=.exe)

TESTIN=./test/in.txt
TESTOUT=./test/out.txt

all:
	$(GHC) $(FLAG) $(SRC) -o $(BIN) -odir '$(OBJDIR)' -hidir '$(HIDIR)'
test:
	$(BIN) $(TESTIN) $(TESTOUT)
	cat $(TESTOUT)
