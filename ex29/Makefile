BUILD = build

.PHONY: all clean
all: $(BUILD)/archive.tar.gz

$(BUILD)/archive.tar.gz: $(BUILD)/output.txt $(wildcard src/*) $(wildcard data/*) | $(BUILD)
	tar -czf $@ src/ data/ $(BUILD)/output.txt

$(BUILD)/output.txt: src/app.py src/helper.py data/input.txt | $(BUILD)
	python3 src/app.py data/input.txt $@

$(BUILD):
	mkdir -p $@

clean:
	rm -rf $(BUILD)
