    git clone https://{Your Personal Access Token}@github.com/{Your username}/{repository address.git}
    cd root/alx-system_engineering-devops
    git init
    mkdir 0x00-shell_permissions
    cd 0x00-shell_permissions
    echo 'My first readme' > README.md
    cat README.md
    git add .
    git commit -m "Commit message"
    git push
    
    NOTE: {} curly brackets is only used to show instructions/commands to follow
    NOTE: {filename} is in bold-italics
    
    cd root/alx-system_engineering-devops/0x00-shell_permissions
    cat > {filename} {pressENTER}
    #!/bin/bash {pressENTER}
    {highlighted text} {pressENTER}
    {press CTRL+D}
    wc -l {filename} {pressENTER}
    head -n 1 {filename} {pressENTER}
    chmod u+x {filename} {pressENTER}
    git add . {pressENTER}
    git commit -m 'write the commit message you want' {pressENTER}
    git push {pressENTER}
    clear {pressENTER}

00. File ***0-iam_betty*** creates a script that switches the current user to the user betty. You should use exactly 8 characters for your command (+1 character for the new line) You can assume that the user betty will exist when we will run your script. `su betty`
```
cat > 0-iam_betty {pressENTER}
#!/bin/bash {pressENTER}
su betty {pressENTER}
{press CTRL+D}
wc -l 0-iam_betty {pressENTER}
head -n 1 0-iam_betty {pressENTER}
chmod u+x 0-iam_betty {pressENTER}
git add . {pressENTER}
git commit -m 'write the commit message you want' {pressENTER}
git push {pressENTER}
clear {pressENTER}
```
  
01. File ***1-who_am_i*** writes a script that prints the effective username of the current user. `whoami`
```
cat > 1-who_am_i {pressENTER}
#!/bin/bash {pressENTER}
whoami {pressENTER}
{press CTRL+D}
wc -l 1-who_am_i {pressENTER}
head -n 1 1-who_am_i {pressENTER}
chmod u+x 1-who_am_i {pressENTER}
git add . {pressENTER}
git commit -m 'write the commit message you want' {pressENTER}
git push {pressENTER}
clear {pressENTER}
```
02. File ***2-bring_me_home*** writes a script that prints all the groups the current user is part of. Note: depending on the user, you will get a different output. `groups`

03. File ***3-new_owner*** writes a script that changes the owner of the file hello to the user betty. `chown betty hello`

04. File ***4-empty*** writes a script that creates an empty file called hello. `touch hello`

05. File ***5-execute*** writes a script that adds execute permission to the owner of the file hello. The file hello will be in the working directory. `chmod u+x hello`

06. File ***6-multiple_permissions*** writes a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello. The file hello will be in the working directory. `chmod ug+x,o+r hello`

07. File ***7-everybody*** writes a script that adds execution permission to the owner, the group owner and the other users, to the file hello. The file hello will be in the working directory. You are not allowed to use commas for this script. `chmod a+x ./ hello`

08. File ***8-James_Bond*** writes a script that sets the permission to the file hello as follows: Owner: no permission at all. Group: no permission at all. Other users: all the permissions. The file hello will be in the working directory You are not allowed to use commas for this script. `chmod 007 hello`

09. File ***9-John_Doe*** writes a script that sets the mode of the file hello to this: The file hello will be in the working directory. You are not allowed to use commas for this script `chmod 753 hello`

10. File ***10-mirror_permissions*** writes a script that sets the mode of the file hello the same as olleh’s mode. The file hello will be in the working directory. The file olleh will be in the working directory. `chmod --reference+olleh hello`

11. File ***11-directories_permissions*** creates a script that ladds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed. `chmod a+x */`

12. File ***12-directory_permissions*** creates a script that creates a directory called my_dir with permissions 751 in the working directory. `mkdir -m 751 my_dir`

13. File ***13-change_group*** writes a script that changes the group owner to school for the file hello. The file hello will be in the working directory. `chgrp school ./hello` `chgrp school hello`

14. File ***100-change_owner_and_group*** writes a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory. `chown vincent:staff *`

15. File ***101-symbolic_link_permissions*** writes a script that changes the owner and the group owner of _hello to vincent and staff respectively. The file _hello is in the working directory. The file _hello is a symbolic link. `chown -h vincent:staff _hello`

16. File ***102-if_only*** writes a script that changes the owner of the file hello to betty only if it is owned by the user guillaume. The file hello will be in the working directory. `chown --from=guillaume betty hello`

17. File ***103-Star_Wars*** writes a script that will play the StarWars IV episode in the terminal. `telnet towel.blinkenlights.nl`
