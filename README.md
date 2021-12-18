Client-Server IPC using named pipes

This is a client program that connects to a given server. The server defines a communication protocol, which the client has to implement by sending properly formulated messages over a communication pipe. The server hosts several electrocardiogram (ECG) data points of 15 patients suffering from various cardiac diseases. The client’s goal, is to obtain these data points by sending properly-formatted messages that the server understands. In addition, the server can send raw files potentially in several segments (i.e., when the file is larger than some internal buffer size). Client has a file transfer functionality and can collect files of arbitrary size using a series of requests/responses.

This implementation uses FIFO (named pipes) for inter process communicaion. Use make to compile. Run the client and it will use fork and exec to run the server as a child process automatically. The files that are to be transfered must be located in the recieved directory and recieved files are stored in the recieved directory. Arguments for client are as follows.

-p patient number (1-15)
	therea are 15 patients on file

-t time (0.00 ~ 60.00) seconds
	request a single time value or leave blank for default 0

-e ecg value 
	1: ecg value 1
	2: ecg value 2
	3: 1000 datapoints from ecg 1
	
-f filename
	desired file name to transfer
	
-c newChannel request
	request the ability to transfer datapoints over a new channel


We obtained the above dataset from physionet.org. 
