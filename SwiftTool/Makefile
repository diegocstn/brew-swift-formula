prefix ?= /usr/local
bindir = $(prefix)/bin


build:
	swift build -c release --disable-sandbox

install: build
	install ".build/release/SwiftTool" "$(bindir)"

uninstall:
	rm -rf "$(bindir)/SwiftTool"

clean:
	rm -rf .build

.PHONY: build install uninstall clean
