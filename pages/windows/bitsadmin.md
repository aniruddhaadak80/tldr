# bitsadmin

> Create, download, or upload Background Intelligent Transfer Service (BITS) jobs, and monitor their progress.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/bitsadmin>.

- Transfer a file in one step:

`bitsadmin /transfer {{job_name}} /download {{https://example.com/file.zip}} {{C:\path\to\file.zip}}`

- Create a job and note the GUID that identifies it:

`bitsadmin /create {{job_name}}`

- Add a file to an existing job:

`bitsadmin /addfile {{job_name}} {{https://example.com/file.zip}} {{C:\path\to\file.zip}}`

- Activate a suspended job in the transfer queue:

`bitsadmin /resume {{job_name}}`

- Display detailed information about a job:

`bitsadmin /info {{job_name}} /verbose`

- Complete a job once its state is `TRANSFERRED`:

`bitsadmin /complete {{job_name}}`

- List all jobs in the transfer queue:

`bitsadmin /list`

- Display help:

`bitsadmin /?`
