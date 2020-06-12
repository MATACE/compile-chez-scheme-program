OBJ = main
LIB = lib

all:
	@echo "Usage:";
	@echo "compile-chez-program <scheme-program.ss> [args ...]";
	@echo "";
	@echo "This will compile a given scheme file and all of its imported libraries";
	@echo "as with (compile-whole-program wpo-file output-file)";
	@echo "see http://cisco.github.io/ChezScheme/csug9.5/system.html#./system:s68";
	@echo "see https://github.com/gwatt/chez-exe";
	@echo "see https://github.com/DeYangLiu/chez-exe";
	@echo "for documentation on compile-whole-program";
	@echo "";
	@echo "Any extra arguments will be passed to the c compiler";
	@echo "";

	./compile-chez-program $(OBJ).ss

clean:
	rm -rf $(OBJ).s $(OBJ).chez $(OBJ).wpo $(OBJ).so $(OBJ)
	rm -rf $(LIB)/*.so $(LIB)/*.wpo
