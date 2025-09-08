# Linux Permissions Commands

## chmod – Change file permissions
chmod 644 file.txt
# Sets permissions so the user can read/write, and others can only read.

chmod 600 secret.txt
# Only the file owner can read/write; others have no access.

chmod 755 script.sh
# User can read/write/execute, others can read and execute.

chmod 700 private.sh
# Only the user can read/write/execute; others have no access.

chmod 664 report.txt
# User and group can read/write, others can only read.

## chown – Change file owner and group
chown alice file.txt
# Changes the owner of file.txt to 'alice'.

chown alice:dev file.txt
# Changes owner to 'alice' and group to 'dev'.

## chgrp – Change group ownership
chgrp dev file.txt
# Changes the group of file.txt to 'dev'.

## umask – Default permissions for new files
umask 022
# New files will have permissions 755 (777 - 022).

umask 077
# New files will have permissions 700 (only user can access).

## id – Show user and group information
id
# Displays user ID (UID), group ID (GID), and groups.

id alice
# Shows details for user 'alice'.

## groups – Show group memberships
groups
# Lists groups for the current user.

groups alice
# Lists groups for user 'alice'.
