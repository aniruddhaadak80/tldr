# VaultCmd

> Create, display, and delete stored credentials.
> See also: `cmdkey`.
> More information: <https://pen2.com/cmd/vaultcmd/>.

- List all vaults and the credentials they contain:

`VaultCmd /list`

- List the properties of a vault:

`VaultCmd /listproperties:"{{Web Credentials}}"`

- List the credentials stored in a vault:

`VaultCmd /listcreds:"{{Windows Credentials}}"`

- List the credential schemas that are available:

`VaultCmd /listschema`

- Synchronize the credential vaults:

`VaultCmd /sync`

- Display help for a specific command:

`VaultCmd /{{command}} /?`
