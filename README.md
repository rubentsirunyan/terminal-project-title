# terminator-project-title
A simple script that echoes project directory basename to use as a title for Terminator tabs

# How to use

1. Clone the repo
	```
    git clone https://github.com/rubentsirunyan/terminator-project-title.git /opt/terminator-project-title
	```
2. Make sure `find_project_root` script is executable
	```
    chmod +x /opt/terminator-project-title/find_project_root
	```	
3. Append ``\e]2;`/path/to/terminator-project-title/find_project_root`\a`` to `PS1` variable in `.bashrc`.
	```
    PS1='[${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\h\[\033[00m\] \[\033[01;34m\]\W\[\033[00m\]]\$ \e]2;`/opt/terminator-project-title/find_project_root`\a'
	```
