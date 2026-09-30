# setquota

> Set disk quotas for users, groups, or projects.
> Block limits are in kibibytes, and accept the `K`, `M`, `G`, and `T` suffixes.
> More information: <https://mankier.com/8/setquota>.

- Set the block and inode limits of a user:

`sudo setquota --user {{user}} {{block_soft_limit}} {{block_hard_limit}} {{inode_soft_limit}} {{inode_hard_limit}} {{path/to/mount_point}}`

- Set the block and inode limits of a group:

`sudo setquota --group {{group}} {{block_soft_limit}} {{block_hard_limit}} {{inode_soft_limit}} {{inode_hard_limit}} {{path/to/mount_point}}`

- Set the block and inode limits of a project:

`sudo setquota --project {{project_id}} {{block_soft_limit}} {{block_hard_limit}} {{inode_soft_limit}} {{inode_hard_limit}} {{path/to/mount_point}}`

- Remove all limits from a user:

`sudo setquota --user {{user}} 0 0 0 0 {{path/to/mount_point}}`

- Set the block grace period of all users on a filesystem, in seconds:

`sudo setquota --edit-period --user {{block_grace_period}} 0 {{path/to/mount_point}}`

- Read the limits to apply from `stdin` in batch mode:

`sudo setquota --batch --user {{path/to/mount_point}}`

- Apply the limits to every filesystem with quotas enabled:

`sudo setquota --all --user {{user}} {{block_soft_limit}} {{block_hard_limit}} {{inode_soft_limit}} {{inode_hard_limit}}`

- Use a specific quota format instead of autodetecting it:

`sudo setquota --format=xfs --user {{user}} {{block_soft_limit}} {{block_hard_limit}} {{inode_soft_limit}} {{inode_hard_limit}} {{path/to/mount_point}}`
