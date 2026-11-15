BUILD_DIR := out

CSV_FILES := $(wildcard data/*.csv)
REPORTS := $(patsubt data/%.csv, out/%.html, $(CSV_FILES))

.PHONY: all clean

all: $(REPORTS)
 
$(BUILD_DIR)/%.html: data/%.csv templates/report.tpl | $(BUILD_DIR)
	reportgen --template templates/report.tpl --input $< --output $@ 

$(BUILD_DIR):
	mkdir -p $(BUILD_DIR)

clean:
	rm -rf $(BUILD_DIR)
