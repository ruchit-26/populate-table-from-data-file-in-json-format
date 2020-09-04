# populate-table-from-data-file-in-json-format
populate table from data file in json format
'''
"""
INSTRUCTIONS
This application will read roster data in JSON format, parse the file, and 
then produce an SQLite database that contains a User, Course, and Member 
table and populate the tables from the data file.
You can base your solution on this code: 
http://www.pythonlearn.com/code/roster.py - this code is incomplete as you
need to modify the program to store the role column in the Member table to
complete the assignment.
Each student gets their own file for the assignment. Download this file 
(https://pr4e.dr-chuck.com/tsugi/mod/sql-intro/roster_data.php?PHPSESSID=ac66d3b8dbd59e2dcfee8c24b15c25b9)
and save it as roster_data.json. Move the downloaded file into the same 
folder as your roster.py program.
Once you have made the necessary changes to the program and it has been run 
successfully reading the above JSON data, run the following SQL command:
SELECT hex(User.name || Course.title || Member.role ) AS X FROM 
    User JOIN Member JOIN Course 
    ON User.id = Member.user_id AND Member.course_id = Course.id
    ORDER BY X
Find the first row in the resulting record set and enter the long string that
looks like 53656C696E613333. 
"""
