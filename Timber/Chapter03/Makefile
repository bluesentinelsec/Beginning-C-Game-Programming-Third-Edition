.PHONY: build

run: build
	cd ../ && ./Timber

build:
	cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -S . -B build
	cmake --build build
	mv build/Timber ../Timber

clean:
	rm -rf build
	rm ../Timber
