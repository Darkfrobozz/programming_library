This is a file that controls the settings of the cargo project.

It is written in TOML (Tom's Obvious, Minimal Language).

The settings file contain a package and a dependencies section.

The package section will list details of the project's edition, name, etc.

The dependencies will specify the [[crate]].
The [[crate]] will then be fetched from crates.io which is like a github for rust.

This settings file can also generate in a locked form. The locked form is the saved handling of all the specific versions you last used. This is to ensure backwards compatibility.

To break past this locked version we can use the cargo command:
	*update*
