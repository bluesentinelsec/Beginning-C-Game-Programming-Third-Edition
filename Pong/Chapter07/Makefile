.PHONY: build

run: build
	cd build && ./Pong


build:
	cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -S . -B build
	cmake --build build
	cp -R fonts build

clean:
	rm -rf build
