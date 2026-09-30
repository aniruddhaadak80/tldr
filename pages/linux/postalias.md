# postalias

> Postfix alias database maintenance utility.
> More information: <https://www.postfix.org/postalias.1.html>.

- Create or rebuild an alias database from a source file:

`sudo postalias {{hash:}}{{/etc/aliases}}`

- Create a database of a specific type:

`sudo postalias {{lmdb:}}{{path/to/aliases}}`

- [q]uery a key in an existing database and write the value to `stdout`:

`postalias -q {{root}} {{hash:/etc/aliases}}`

- [d]elete a key from an existing database:

`sudo postalias -d {{root}} {{hash:/etc/aliases}}`

- Read entries from `stdin` and add them to an existing database without truncating it:

`sudo postalias -i {{hash:}}{{path/to/aliases}}`

- Retrieve all database entries as `key: value` lines:

`postalias -s {{hash:/etc/aliases}}`

- Read the `main.cf` configuration file from a non-default directory:

`sudo postalias -c {{path/to/config_directory}} -q {{root}} {{hash:/etc/aliases}}`
