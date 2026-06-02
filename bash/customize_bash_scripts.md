# Add color and time to line
```sh 
 cp ~/.bashrc ~/.bashrc.bak 2>/dev/null || true && { echo -e "\n# Custom additions with color156 commands and color188 items\nYELLOW='\\033[1;33m'\nNC='\\033[0m'\nalias ll='ls --color=auto'\nalias la='ls -A --color=auto'\nalias grep='grep --color=auto'\nLS_COLORS=\"di=01;38;5;188:ln=01;38;5;156:so=01;38;5;156:pi=01;38;5;156:ex=01;38;5;156:bd=01;38;5;156:cd=01;38;5;156:su=01;38;5;156:sg=01;38;5;156:tw=01;38;5;156:ow=01;38;5;156\"\; export LS_COLORS\nPS1='\${debian_chroot:+(\$debian_chroot)}\\[\\033[01;32m\\]\\u@\\h\\[\\033[00m\\]:\\[\\033[01;34m\\]\\w\\[\\033[00m\\] ${YELLOW}[$(date +%H:%M:%S)]${NC}\$ '" >> ~/.bashrc && source ~/.bashrc; }
```

# Exsmple of terminal colors
```sh 
for i in {0..255}; do printf "\x1b[38;5;${i}mcolor%-5i\x1b[0m" $i ; if ! (( ($i + 1 ) % 8 )); then echo ; fi ; done
```
