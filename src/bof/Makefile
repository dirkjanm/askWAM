CC := x86_64-w64-mingw32-gcc

CFLAGS := -c -Os -Wall -Wextra -ffreestanding \
          -fno-stack-protector -fno-asynchronous-unwind-tables \
          -fno-tree-loop-distribute-patterns \
          -DUNICODE -D_UNICODE

OBJ := bin/Release/askwam_bof.x64.o

$(OBJ): askwam_bof.c beacon_min.h
	mkdir -p $(dir $@)
	$(CC) $(CFLAGS) -o $@ $<

clean:
	rm -rf bin

.PHONY: clean
