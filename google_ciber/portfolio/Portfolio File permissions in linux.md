2024-09-28 17:17

Status:

Tags:
[[Cyber security]]

# Portfolio File permissions in linux

## Project description

We were tasked to examine existing permissions on the file system, and check if said permissions match the authorization that should be given, if they don't match we need to modify the permissions to authorize the appropriate users and remove the rest.



## Check file and directory details

in order to check the file we first move to it using `cd /home/researcher2/projects` once we are inside of the file we will check we used `ls -la` in order to show the directory's contents and check the permissions, we found several files and a folder had the wrong permissions.

## Describe the permissions string

On files the string starts with a - and on directories it starts with a d, the string is divided into 3 permission groups each with 3 possible permissions which are Read, Write, Execute.

- Read: For files allows the user to view and read the contents of a file.
  For directories allows the user to see the folder and its contents.
  
- Write: For files allows the user to modify or edit a file's content's.
  For directories allows the user to rename,create or delete files/folders in the directory.

- Execute: For files allows the user to run the file as a program or script.
  For directories allows the user to enter the directory and access files within it (even if they cant list the directory's content).
and the groups are User, Group, Others.

- User: Refers to the user who owns the file, usually it's the file or folder creator but ownership can be transferred.
- Group: Refers to the group of users who are assigned a shared access to the file or folder.
- Others: Refers to all other users who are not the owner and do not belong to the group.

## Change file permissions

In order to fix the permissions on project_k.txt we used `chmod 664` in order to adjust the permissions of that file making it read/write for user and group and only read for others.

We noticed that the file project_m.txt needed more restrictive permissions so we changed them by using `chmod 600` in order to make it only read/write for the user.

## Change file permissions on a hidden file

since the file project_x.txt is a hidden file it can only be read by the user and groups but they shouldn't be able to write or execute it, to achieve that we used `chmod 437` in order to make it only readable by the user & group only.

## Change directory permissions

We also noticed that the directory drafts isn't using the correct permissions only the owner: "researcher2" should be able to execute said directory, in order to fix that we used `chmod 700` in order to make it read/write/executable for the owner.
## Summary

3 files and a directory were in need of correct permissions that were successfully given and will allow the project to continue to be secure following the principle of least privilege (PoLP), ensuring only users who are authorized can access their respective files.


References 