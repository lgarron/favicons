all: favicon.ico

SOURCE_FULL = alg.cubing.net.png

INTERMEDIATE_1X = build/alg.cubing.net.png
INTERMEDIATE_2X = build/alg.cubing.net@2x.png

$(INTERMEDIATE_1X): $(SOURCE_FULL)
	convert $(SOURCE_FULL) -scale 16 $(INTERMEDIATE_1X)

$(INTERMEDIATE_2X): $(SOURCE_FULL)
	convert $(SOURCE_FULL) -scale 32 $(INTERMEDIATE_2X)

########

SOURCES = $(INTERMEDIATE_1X) $(INTERMEDIATE_2X)

favicon.ico: $(SOURCES)
	convert $(SOURCES) favicon.ico
