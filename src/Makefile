# Compilation
SOURCES = $(wildcard *.c)
OBJECTS = $(patsubst %.c,$(OUT)/%.o,$(SOURCES))

.PHONY: all clean

all: $(OBJECTS)

$(OUT)/%.o: %.c
	$(MKD) $(OUT)
	$(CC) $(CFLAGS) -I $(INC_DIR) -c $< -o $@

clean:
	$(RMD) $(OUT) %.o
