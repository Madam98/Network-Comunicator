# Network-Comunicator

### Description
An application that allows users to join a chat room and enables them to exchange messages. The user application was developed in Java, the server in C.

### Key features of the project
- learning about sockets, descriptor management, TCP communication basics
- creating a java client that responds to specific user commands
- asynchronous joining of multiple users to a chat room
- basic message synchronization between all users

### Server instructions
Usage:
[command]:[arguments].
IT IS IMPORTANT THAT THERE IS NO SPACE BETWEEN THE COMMAND A ":"!

Command legend (for the server):
- [add] - add a new user and create his folder, assign an appropriate path for the user (should be called only once when creating)
- [touch] - add a new file named arguments
- [share] - send a file descriptor to share with some users
- [delete] - delete a file with a given name
- [copy] - copy a file with a given name and add a prefix "COPY_".
- [newname] - change the name of the file. To change the name it should be sent as newname:name_file_1 > name_file_2 (SPACES BEFORE > AND AFTER ARE MUST!).
- [Enter] - open the file with the given name. Assigns a descriptor to the client structure
- [modifiy] - send a character to the file and save it
- [close] - close the file
