# dyld_info

> Display the information that `dyld` uses to load a Mach-O binary.
> More information: <https://keith.github.io/xcode-man-pages/dyld_info.1.html>.

- [L]ist the dylibs that a binary is linked against:

`dyld_info -linked_dylibs {{path/to/binary}}`

- Display the p[l]atform that a binary was built for:

`dyld_info -platform {{path/to/binary}}`

- Display all [s]egments and sections with size information:

`dyld_info -segments {{path/to/binary}}`

- Display all [e]xported symbols:

`dyld_info -exports {{path/to/binary}}`

- Display all [i]mported symbols:

`dyld_info -imports {{path/to/binary}}`

- Display a simple table of [f]ixup locations:

`dyld_info -fixups {{path/to/binary}}`

- Display the [u]UID of a binary:

`dyld_info -uuid {{path/to/binary}}`

- Only display information for a specific [a]rchitecture of a universal binary:

`dyld_info -arch {{arch_name}} -exports {{path/to/binary}}`
