[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-f059dc9a6f8d3a56e377f745f24479a46679e63a5d9fe6f495e02850cd0d8118.svg)](https://classroom.github.com/online_ide?assignment_repo_id=5569735&assignment_repo_type=AssignmentRepo)
# PA1: Client-Server IPC using named pipes

In this assignment, you will write a client program that connects to a given server. The server defines a communication protocol, which the client has to implement by sending properly formulated messages over a communication pipe. The server hosts several electrocardiogram (ECG) data points of 15 patients suffering from various cardiac diseases. The client’s goal, thereby your goal, is to obtain these data points by sending properly-formatted messages that the server understands. In addition, the server can send raw files potentially in several segments (i.e., when the file is larger than some internal buffer size). Your client must implement this file transfer functionality as well such that it can collect files of arbitrary size using a series of requests/responses.  See project document on Canvas for more details.

We obtained the above dataset from physionet.org. 
