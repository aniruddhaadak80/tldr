# postmap

> Postfix lookup table management utility.
> More information: <https://www.postfix.org/postmap.1.html>.

- Create or rebuild a lookup table from a source file:

`sudo postmap {{hash:}}{{/etc/postfix/virtual}}`

- Create a lookup table of a specific type:

`sudo postmap {{lmdb:}}{{path/to/virtual}}`

- [q]uery a key in an existing lookup table and write the value to `stdout`:

`postmap -q {{user@example.com}} {{hash:/etc/postfix/virtual}}`

- [d]elete a key from an existing lookup table:

`sudo postmap -d {{user@example.com}} {{hash:/etc/postfix/virtual}}`

- Read entries from `stdin` and add them to an existing table without truncating it:

`sudo postmap -i {{hash:}}{{path/to/virtual}}`

- Retrieve all table entries as `key value` lines:

`postmap -s {{hash:/etc/postfix/virtual}}`

- Read the `main.cf` configuration file from a non-default directory:

`sudo postmap -c {{path/to/config_directory}} -q {{user@example.com}} {{hash:/etc/postfix/virtual}}`
