```
-----------------------------------------
 ______     _______    ______      _____
(_____ \   (_______)  |  ___ \    / ___ \
 _____) )   _____     | | _ | |  | |   | |
(_____ (   |  ___)    | || || |  | |   | |
      | |  | |_____   | || || |  | |___| |
      |_|  |_______)  |_||_||_|   \_____/
                                          
------------------------------------------
```

REMO MODE IS A ALIAS AUTOMATION TOOL

WE FORGOT WE CAN CUSTOMIZE A LOT OF OUR WORK BY USING ALIAS AND NOT ITS EVEN MORE EASY FOR YOU

![image](https://github.com/ReubenReny03/remo_mode/assets/91770238/69719100-3379-467d-8b4c-9ba5fdaf3e35)

STEP 1 : run the installremo file → source installremo

**AUTOMATIC REBOOT**

STEP 2 : use remo_edit to add new alias

**AND ENJOY : )**

Hi all, Remo Mode is a feeling to make your linux life feel more special my goal is to make you feel happy with linux by given	ing it a touch of Remo.

Hi, I am Remo and you can rename this project and make your own version of it and add new things which are really cool.


What is inside the install.sh?

Add remo_mode alias to .bashrc so that you can turn it on when needed.


```
NEW_LINE='alias remo_mode="source ~/.todo"' #? Add alias to .bashrc

# Append the line to ~/.bashrc
echo $NEW_LINE >> ~/.bashrc

echo "Line added to ~/.bashrc: $NEW_LINE"
```


Add .todo list of all the things which remo_mode can do and how will it to 

Write the file contents and reboot 


```
NEW_FILE="$HOME/.remo_todo"
MULTILINE_CONTENT=$(cat <<EOM                                                                        
notify-send REMO_IS_BACK
alias file_dir="thunar"
alias exams_f="cd ~/Documents/EXAMS/IA_1/"
alias remo-help="cat ~/.remo_on"
alias class-wt="firefox https://classroom.google.com/c/NTU0NTQwMDQ4OTQ1"
alias remo_edit="nano ~/.remo_todo
cat ~/.remo_on
EOM
)

touch "$NEW_FILE"
echo "$MULTILINE_CONTENT" > "$NEW_FILE"
echo "New file created: $NEW_FILE"
echo "Content added:"

reboot
```


If you ever want to edit the file and add new shortcut alias then just type remo_edit

And add :
```
alias {name_you want}=”{command you want to run}”
```
