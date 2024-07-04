MultiThreaded File Server and Logging Application
A Java implementation of a multi-threaded file server and logging application, enabling clients to download files using a terminal user interface.

Features
**MultiThreaded**: Capable of handling multiple clients simultaneously.
**BlockingQueue**: Implements a multiple producer/one consumer model.
**Documentation**: Includes comprehensive Javadocs.
**UML** Diagrams: Provides 2 UML diagrams for better understanding.
**Robustness**: Operates with one, no, or two parameters.

User Guide
Installation
To run the application, navigate to the directory containing the oop.jar file and use the following commands:
Start the server
`$ java -cp .:./oop.jar ie/gmit/sw/server/ServerRunner 7777 path/to/my/files`

Start the client
`$ java -cp .:./oop.jar ie/gmit/sw/server/ClientRunner`

Upon starting the client, you will be presented with a menu of options:

Connect to server
Print all files (requires connection)
Download file (requires connection)
Quit
Features and Functionalities
Connect
The client parses settings from an XML file using XMLParser. Once parsed, the client attempts to connect to the server via sockets. A successful connection will notify the client, enabling further operations.

List All Files
Requires a connection. The client sends a ListFileRequest to the server, which responds with a list of available files.

Download File
The client prompts for a filename and attempts to retrieve it from the server. If the file is found, the server transfers the file to the client. If unsuccessful, the server informs the client and returns to the menu.

API
To access the API, navigate to /api/currencyName (e.g., /api/sdc) for various currency information.
