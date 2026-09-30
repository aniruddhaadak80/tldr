# vtool

> Display and edit the build and source version numbers of Mach-O files.
> More information: <https://keith.github.io/xcode-man-pages/vtool.1.html>.

- Display the build and source versions of a binary:

`vtool -show {{path/to/binary}}`

- Display only the build versions of a binary:

`vtool -show-build {{path/to/binary}}`

- Display only the source version of a binary:

`vtool -show-source {{path/to/binary}}`

- Set the minimum OS and SDK version for a platform, writing the result to a new file:

`vtool -set-build-version {{platform}} {{minos_version}} {{sdk_version}} -output {{path/to/output}} {{path/to/binary}}`

- Set the source version of a binary, writing the result to a new file:

`vtool -set-source-version {{version}} -output {{path/to/output}} {{path/to/binary}}`

- Remove the source version of a binary, writing the result to a new file:

`vtool -remove-source-version -output {{path/to/output}} {{path/to/binary}}`

- Only operate on a specific architecture of a universal binary:

`vtool -arch {{arch}} -show-build {{path/to/binary}}`

- Display the usage of `vtool`:

`vtool -help`
