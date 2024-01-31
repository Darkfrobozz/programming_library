Cargo is the rust project creation and organization tool.

This tool is built to remove a lot of the hassle that comes from code that work from a lot of dependencies.

Cargo has several commands tied to it:
	- fmt, This runs a rust style check
	- new <1>, 
	This creates a new cargo project, the 1 param is the name of the project.
	It also initializes a git repo, a src directory and a Cargo.toml file.
	The [[cargo_toml]] file are the settings for cargo. TOML??
	- [[build]], creates binaries in a target directory and a cargo.lock file
	- run, builds (if necessary) and then runs the target bin
	- clean, removes target
	- check, quickly checks if the code is compilable