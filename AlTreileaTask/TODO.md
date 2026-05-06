📋 FTP Exercise - TODO List
✅ IMPLEMENTED (Backend & Frontend)
Server-Side (server.py)
 FTP Server with socket communication
 User authentication (default: student/1234)
 files/ directory management (auto-create)
 Command processing and response handling
 create_file: Store file on server
 upload: Receive file from client
 rename_file: Server returns "not implemented" message for students
 read_file: Server returns "not implemented" message for students
 download: Server returns "not implemented" message for students
 edit_file: Server returns "not implemented" message for students
 see_file_operation_history: Server returns "not implemented" message for students
 list_files: Show all files on server
 logout: End user session
 Multi-threaded client handling
 JSON protocol for communication
Client-Side (client.py)
 Connection to FTP server
 login: Authenticate with username/password
 create_file(): Create file locally with name, extension, and content
 upload(): Send local file to server
 rename_file(): Send request to server and display server message
 read_file(): Send request to server and display server message
 download(): Send request to server and display server message
 edit_file(): Send request to server and display server message
 see_file_operation_history(): Send request to server and display server message
 list_files(): Display files on server
 logout(): Disconnect from server
 disconnect(): Close connection
 Menu interface with all options
 Local files directory management (local_files/)
🚀 TO IMPLEMENT BY STUDENTS
All these methods are in client.py and marked with [STUDENT] in the menu.

1. rename_file()
 Ask user for OLD filename
 Ask user for NEW filename
 Send rename_file command to server with old_name and new_name
 Display success/error response
2. read_file()
 Get list of files from server
 Ask user to select a file
 Send read_file command to server
 Display file content in console
3. download()
 Get list of files from server
 Ask user to select a file
 Send download command to server
 Save received content to local_files/ directory
 Confirm file was saved
4. edit_file()
 Get list of files from server
 Ask user to select a file
 Ask user for new content
 Send edit_file command to server with filename and new content
 Display success/error response
5. see_file_operation_history()
 Get list of files from server
 Ask user to select a file
 Send see_file_operation_history command to server
 Display the server response message
 Students must implement file history tracking on the server (create, edit, rename, etc operations)
📁 Project Structure
Seminar 10/
├── server.py
├── client.py
├── TODO.md
├── files/
└── local_files/
🔐 Default Credentials
Username: student
Password: 1234