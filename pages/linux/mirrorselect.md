# mirrorselect

> Select Gentoo source and rsync mirrors.
> More information: <https://wiki.gentoo.org/wiki/Mirrorselect>.

- Interactively select source mirrors and update `GENTOO_MIRRORS`:

`sudo mirrorselect -i`

- Interactively select source mirrors located in a specific country:

`sudo mirrorselect -i -c "{{United States (USA)}}"`

- Test the 3 fastest servers by downloading 100K from each:

`mirrorselect -s3 -b10 -D`

- Interactively select an rsync mirror:

`sudo mirrorselect -i -r`

- Only consider mirrors served over HTTPS:

`mirrorselect -i -S`

- Only consider mirrors reachable over IPv4:

`mirrorselect -i -4`

- Only consider mirrors in a specific region:

`mirrorselect -i -R "{{North America}}"`

- Display the program version:

`mirrorselect --version`
