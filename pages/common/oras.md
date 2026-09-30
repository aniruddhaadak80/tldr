# oras

> OCI registry client for managing artifacts, images, and packages.
> Artifacts are addressed as `[registry/]repository[:tag|@digest]`.
> More information: <https://oras.land/docs/commands/use_oras_cli/>.

- Log in to a registry:

`oras login {{registry}}`

- Log out from a registry:

`oras logout {{registry}}`

- Push a directory to a registry as an artifact:

`oras push {{path/to/directory}} {{registry/repository:tag}}`

- Pull an artifact into a specific directory:

`oras pull --output {{path/to/directory}} {{registry/repository:tag}}`

- Attach a file to an existing artifact:

`oras attach --artifact-type {{application/example}} {{registry/repository:tag}} {{path/to/file}}`

- List the tags of a repository:

`oras repo tags {{registry/repository}}`

- Discover the referrers of a manifest:

`oras discover {{registry/repository:tag}}`

- Display version information:

`oras version`
