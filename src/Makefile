CXX = g++
CXXFLAGS = -std=c++14
OBJECTS = main.o quadris.o block.o cell.o board.o textdisplay.o subject.o graphicsdisplay.o window.o
DEPENDS = ${OBJECTS:.o=.d}
EXEC = quadris

${EXEC}: ${OBJECTS}
	${CXX} ${CXXFLAGS} ${OBJECTS} -o ${EXEC} -lX11

-include ${DEPENDS}

clean:
	-rm *.o quadris
