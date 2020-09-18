# MyTunes-Library
MyTunes Library program gets the user to read and sort unfiltered data of songs and filter them using user preferences. The program demonstrates sorting algorithms. Runs on Linux operating system through a command shell.

Compiler command: 
	 type: 'make'
	 The command will generate the executable and object files for the
	 assignment.
	 The name of the executable file is: musiclib

To run the program:
       	 './musiclib'

Demonstrating the test cases:

	      	  //Test add Commands
//add recording
add -r 103 "Beatles For Sale" "Beatles" "George Martin" 1964
//add song
add -s 1001 "Misery" "Paul McCartney, John Lennon"
//add track
add -t 100 1000 1
//add users
add -u ajones "Anne Jones"
//add playlists
add -p ldnel "Driving Songs"
//add playlist tracks
add -l ldnel "Driving Songs" 1001 

       	     	   //Test delete Commands
delete -s song_id
delete -s song_id -p playlist_name -u user_name 
delete -Global -s song_id -p playlist_name -u user_name
delete -r recording_id 
delete -u user_id
delete -p playist_name -u user_id 
delete -t song_id recording_id

       	  	  //Test show Commands
show songs
show users
show playlists -u user_id
show songs -u user_id -p playlist_name
show recordings
show tracks

		  //Test UI SHELL COMMANDS (start with a dot):
//not included in this test:
//.quit --because it will terminate the app
//.help --not meant to be scripted
//.log save filename --can be done manually
//.read --proved by being able to run this script

		 //Test Logs
.log clear //clear the logs
.log start //begin logging commands only
.log start_output //begin logging output only
.log start_both  //begin logging commands and output
.log stop //stop logging
.log show //display current log contents on console

     	  	 //Test Comments
//This is a comment.


Note: There is a seperate file with the name: cmdscript.txt
The same information is avaiable in it, since it may be easier to run the test
cases. 
