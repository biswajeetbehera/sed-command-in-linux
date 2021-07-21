# sed-command-in-linux

# To replace any particular word with a new one from any line from a file in linux give below command
sed  -i's/word name to be replaced/new word name/g' file name.

# To remove empty lines from a file, use below command
sed -i '/^$/d' file name

#To remove the first line from any file give below comand
sed -i '1d' file name

# similarly to remove the second line from a file use below command
sed -i '1,2d' file name
# to remove tabs and replace it with space use below command
sed -i 's/\t/ /g' file name
# supppose there are 18 lines in a file. you want to remove the from 1 to 11 and show only 12 to 18, then use below command
sed -i -n 12,18p filename
# supppose there are 18 lines in a file. you want to show the from 1 to 11 and remove only 12 to 18, then use below command
sed -i 12,18d file name
