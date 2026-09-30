# xorriso

> Create, load, manipulate, and write ISO 9660 filesystem images.
> Note: this program is also installed as `xorrisofs`, `xorrecord`, and `osirrox`.
> More information: <https://mankier.com/1/xorriso>.

- Create an ISO image from a directory, using `mkisofs` emulation:

`xorriso -as mkisofs -o {{path/to/image.iso}} {{path/to/directory}}`

- List the contents of an ISO image file:

`xorriso -indev {{path/to/image.iso}} -ls`

- List the contents of a directory inside an ISO image file:

`xorriso -indev {{path/to/image.iso}} -ls {{/path/inside/image}}`

- Extract a file or directory tree from an ISO image file to disk:

`xorriso -osirrox on -indev {{path/to/image.iso}} -extract {{/path/inside/image}} {{path/to/destination}}`

- Print the size of the ISO image that would be written, without writing it:

`xorriso -as mkisofs -print-size {{path/to/directory}}`

- Write an ISO image file to a blank optical drive, using `cdrecord` emulation:

`xorriso -as cdrecord -v dev={{/dev/sr0}} blank=as_needed {{path/to/image.iso}}`

- Display the program name and version:

`xorriso -version`
