BUILD_DIR := build
CC := gcc

.PHONY: all clean

all: $(BUILD_DIR)/calculator

$(BUILD_DIR)/calculator: $(BUILD_DIR)/main.o $(BUILD_DIR)/math.o
	$(CC) $^ -o $@

$(BUILD_DIR)/main.o: src/main.c src/math.h | $(BUILD_DIR)
	$(CC) -c $< -o $@

$(BUILD_DIR)/math.o: src/math.c src/math.h | $(BUILD_DIR)
	$(CC) -c $< -o $@

$(BUILD_DIR):
	mkdir -p $@

clean:
	rm -rf $(BUILD_DIR)
