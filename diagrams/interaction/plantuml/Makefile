SRC            != ls *.uml
INC            != ls *.iuml
IMG             = ${SRC:.uml=.png}
PLANTUML       ?= plantuml

all: ${IMG}

.SUFFIXES: .uml .png
.uml.png: ${INC}
	${PLANTUML} $<

.PHONY: clean
clean:
	rm -f ${IMG}
