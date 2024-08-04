.PHONY: build

run: build
	cd ../ && ./Timber

enhanced: build
	cd ../ && ./Timber_Enhanced

build:
	cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -S . -B build
	cmake --build build
	mv build/Timber ../Timber
	mv build/Timber_Enhanced ../Timber_Enhanced

clean:
	rm -rf build
	rm ../Timber
