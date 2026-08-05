
CXXFLAGS ?= -O2 -Wall

bc250memcfg: main.cpp
	$(CXX) $(CXXFLAGS) -fwhole-program -o "$@" "$<"

all: bc250memcfg

install: bc250memcfg
	mkdir ${DESTDIR}/${PREFIX}/bin
	install -m0755 -t "${DESTDIR}/${PREFIX}/bin/" bc250memcfg

.PHONY: all clean install
