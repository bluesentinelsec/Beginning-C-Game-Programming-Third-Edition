.PHONY: build

build:
	cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -S . -B build
	cmake --build build
	mv build/Timber ./Timber

run: build
	./Timber

clean:
	rm -rf build
	rm Timber
