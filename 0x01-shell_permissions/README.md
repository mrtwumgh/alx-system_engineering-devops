# 0x01. Shell, permissions
-   Allowed editors:  `vi`,  `vim`,  `emacs`
-   All your scripts will be tested on Ubuntu 20.04 LTS

### 0-iam_betty
a script that switches the current user to the user `betty`.

### 1-who_am_i
a script that prints the effective username of the current user.

### 2-groups
a script that prints all the groups the current user is part of.

### 3-new_owner
a script that changes the owner of the file `hello` to the user `betty`.

### 4-empty
a script that creates an empty file called `hello`.

### 5-execute
a script that adds execute permission to the owner of the file `hello`.

### 6-multiple_permissions
a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file `hello`.

### 7-everybody
a script that adds execution permission to the owner, the group owner and the other users, to the file `hello`

### 8-James_Bond
a script that sets the permission to the file  `hello`  as follows:

-   Owner: no permission at all
-   Group: no permission at all
-   Other users: all the permissions

### 9-John_Doe
a script that sets the mode of the file  `hello`  to this:

```
-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
```

### 10-mirror_permissions
a script that sets the mode of the file  `hello`  the same as  `olleh`’s mode.

-   The file  `hello`  will be in the working directory
-   The file  `olleh`  will be in the working directory

```
julien@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 julien julien 42 Sep 20 14:45 10-mirror_permissions
-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
-rw-rw-r-- 1 julien julien  0 Sep 20 14:43 olleh
julien@ubuntu:/tmp/h$ ./10-mirror_permissions 
julien@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 julien julien 42 Sep 20 14:45 10-mirror_permissions
-rw-rw-r-- 1 julien julien 23 Sep 20 14:25 hello
-rw-rw-r-- 1 julien julien  0 Sep 20 14:43 olleh
julien@ubuntu:/tmp/h$ 

```

Note: the mode of  `olleh`  will not always be 664. Make sure your script works for any mode.

### 11-directories_permissions
a script that adds execute permission to all subdirectories of the  **current directory**  for the owner, the group owner and all other users.

Regular files should not be changed.

### 12-directory_permissions
a script that creates a directory called `my_dir` with permissions 751 in the working directory.

### 13-change_group
a script that changes the group owner to `school` for the file `hello`

### 100-change_owner_and_group
a script that changes the owner to `vincent` and the group owner to `staff` for all the files and directories in the working directory.

### 101-symbolic_link_permissions
a script that changes the owner and the group owner of  `_hello`  to  `vincent`  and  `staff`  respectively.

-   The file  `_hello`  is in the working directory
-   The file  `_hello`  is a symbolic link

### 102-if_only
a script that changes the owner of the file  `hello`  to  `betty`  only if it is owned by the user  `guillaume`.

-   The file  `hello`  will be in the working directory

### 103-Star_Wars
a script that will play the StarWars IV episode in the terminal.
