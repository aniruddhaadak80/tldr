# install_name_tool

> Change the install names of dynamic shared libraries and the rpaths of Mach-O binaries.
> More information: <https://keith.github.io/xcode-man-pages/install_name_tool.1.html>.

- Change the install name of a shared library:

`install_name_tool -id {{new_name}} {{path/to/shared_library.dylib}}`

- Change a dependent shared library install name:

`install_name_tool -change {{old_name}} {{new_name}} {{path/to/binary}}`

- Add an rpath to a binary:

`install_name_tool -add_rpath {{@loader_path/../lib}} {{path/to/binary}}`

- Delete an rpath from a binary:

`install_name_tool -delete_rpath {{@loader_path/../lib}} {{path/to/binary}}`

- Change an existing rpath of a binary:

`install_name_tool -rpath {{old_path}} {{new_path}} {{path/to/binary}}`
