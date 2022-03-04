    git clone https://{Your Personal Access Token}@github.com/{Your username}/{repository address.git}
    cd root/alx-system_engineering-devops
    git init
    mkdir 0x00-shell_basics
    cd 0x00-shell_basics
    echo 'My first readme' > README.md
    cat README.md
    git add .
    git commit -m "Commit message"
    git push
    
    NOTE: {} curly brackets is only used to show instructions/commands to follow
    NOTE: {filename} is in bold-italics
    
    cd root/alx-system_engineering-devops/0x00-shell_basics
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
    
00. File ***0-current_working_directory*** writes a script that prints the absolute path name of the current working directory. `pwd`
```
cat > 0-current_working_directory {pressENTER}
#!/bin/bash {pressENTER}
pwd {pressENTER}
{press CTRL+D}
chmod u+x 0-current_working_directory {pressENTER}
git add . {pressENTER}
git commit -m 'write the commit message you want' {pressENTER}
git push {pressENTER}
clear {pressENTER}
```
  
01. File ***1-listit*** displays the contents list of the current directory. `ls`
```
cat > 1-listit {pressENTER}
#!/bin/bash {pressENTER}
ls {pressENTER}
{press CTRL+D}
chmod u+x 1-listit {pressENTER}
git add . {pressENTER}
git commit -m 'write the commit message you want' {pressENTER}
git push {pressENTER}
clear {pressENTER}
```
02. File ***2-bring_me_home*** writes a script that changes the working directory to the user’s home directory. `cd ~`

03. File ***3-listfiles*** displays current directory contents in a long format. `ls -l`

04. File ***4-listmorefiles*** displays current directory contents, including hidden files (starting with .) Using the long format. `ls -la`

05. File ***5-listfilesdigitonly*** displays current directory contents in long format, with user and group IDs displayed numerically and hidden files. `ls -lna`

06. File ***6-firstdirectory*** creates a script that creates a directory named my_first_directory in the /tmp/ directory. `mkdir /tmp/my_first_directory`

07. File ***7-movethatfile*** moves the file betty from /tmp/ to /tmp/my_first_directory. `mv /tmp/betty /tmp/my_first_directory`

08. File ***8-firstdelete*** deletes the file betty. The file betty is in /tmp/my_first_directory. `rm /tmp/my_first_directory/betty`

09. File ***9-firstdirdeletion*** deletes the directory my_first_directory that is in the /tmp directory. `rmdir /tmp/my_first_directory`

10. File ***10-back*** writes a script that changes the working directory to the previous one. `cd -`

11. File ***11-lists*** writes a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format. `ls -al . .. /boot`

12. File ***12-file_type*** writes a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script. `file /tmp/iamafile`

13. File ***13-symbolic_link*** creates a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory. `ln -s bin/ls __ls__`

14. File ***14-copy_html*** creates a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory. You can consider that all HTML files have the extension .html `cp -nu *.html ..`

15. File ***100-lets_move*** creates a script that moves all files beginning with an uppercase letter to the directory /tmp/u. You can assume that the directory /tmp/u will exist when we will run your script. `mv [[:upper:]]* /tmp/u`

16. File ***101-clean_emacs*** creates a script that deletes all files in the current working directory that end with the character ~. `rm *~`

17. File ***102-tree*** creates a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory. You are only allowed to use two spaces (and lines) in your script, not more. `mkdir -p welcome/to/school`

18. File ***103-commas*** writes a command that lists all the files and directories of the current directory, separated by commas (,). Directory names should end with a slash (/). Files and directories starting with a dot (.) should be listed. The listing should be alpha ordered, except for the directories . and .. which should be listed at the very beginning. Only digits and letters are used to sort; Digits should come first. You can assume that all the files we will test with will have at least one letter or one digit. The listing should end with a new line. `ls -pamv`

19. File ***school.mgc*** reates a magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset 0.
```
cat > school.mgc {pressENTER}
0 string SCHOOL School data {pressENTER}
!:mime School {pressENTER}
chmod u+x school.mgc {pressENTER}
file -C -m school.mgc {pressENTER}
git add . {pressENTER}
git commit -m 'write the commit message you want' {pressENTER}
git push {pressENTER}
```
