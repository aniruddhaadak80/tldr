# otool

> Display parts of object files, libraries and Mach-O binaries.
> More information: <https://keith.github.io/xcode-man-pages/otool.1.html>.

- [L]ist the shared libraries that a binary uses:

`otool -L {{path/to/binary}}`

- Display the [l]oad commands of a binary:

`otool -l {{path/to/binary}}`

- [D]isplay the install name of a shared library:

`otool -D {{path/to/shared_library.dylib}}`

- Display the universal [f]at headers of a binary:

`otool -f {{path/to/binary}}`

- Display the table of contents of a dynamically linked shared library:

`otool -S {{path/to/shared_library.dylib}}`

- Disassemble the text section of a binary:

`otool -v -t {{path/to/binary}}`

- Only operate on a specific architecture of a universal binary:

`otool -arch {{arch_type}} -L {{path/to/binary}}`

- Display the version of `otool`:

`otool --version`
