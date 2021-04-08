# SquidNet
A highly functional Botnet with security, powerful bot scripts, and the ability to set up remote access to it with admin scripts. It is mainly using TCP for regular bots, but it can use SSH when logging into SSH Servers.

# Features:
Security - Has a Username and Password that the user is able to configure, to set up remote connections.

Web-Interface - Ability to view connections and general info about the server via a webpage

Option-Parsing - Re-usability and having the ability to configure the server with only one cmd command.

Bots - Compromised Bots infected with the Bot script will connect to the server(if configured correctly), and are able to do many different things.

Remote-Connections - Ability to set-up remote connections with admins, so that the server can also be used remotely via an admin.

SSH Compatability - The botnet can also take control of SSH Servers.

Logging - The server is logged, and server errors can be checked there.

# Security:

The Botnet will be able to determine whether a bot is a bot or not. There is a custom command for being recognized by the botnet. If that command is not recieved, the incoming connection will be closed, and they will be kicked. If they do enter the correct command, they will be recognized as a proper client of the Botnet. If an admin is connecting to the Botnet, they will send the login command to the server, and also send the command that allows them access. They will need to enter the correct username or password, otherwise they will be kicked and the server will be warned. During password configuration(sorry for going a little off topic), the provided username will be put in a txt file, as well as the password. However, this password will first be hashed with the md5 hashing algorythm for increased security. Back to the admins connections, the username and password will be checked with the txt file with the correct credentials. The password in the command will first be hashed, and it will be checked with what is in the text file. If the username and password are correct, they will be granted access to the server.

Example of the Admin-File:

![adminfile](/ex1.png)

# Web-Interface

The Botnet has a web-interface for when the user wants to see the connections in a more simpler format. The web-interface will be able to show the connections in a table, where it is much easier to read, as well as showing information about them. In the tables, you are able to see the hostname of who is connected, the IP Address, the username of the connection, the source port(good for differentiate between duplicate connections), as well as the os. The main connections are listed in the first table, and the admin connections are listed in the second. For the SSH Connections, those are listed in the 3rd table. They will have the hostname first, then the IP Address, and finally the password of the SSH Server. Then there will be some other information about the configured variables in the Botnet. These include where the log file is located, the IP and Port used to connect to the Botnet, the admin login info, Encryption Key for encrypting files on the bots, and also the bruteforcing password-list for ssh connections. It doesn't look too great, as I am not very knowledgeable when it comes to HTML. 

Example of the Web-Interface:

![webinterface](/ex2.png)

# Option-Parsing

(Writing in progress)

# Bots

(Writing in progress)

# Remote-Connections

(Writing in progress)

# SSH-Compatibility

(Writing in progress)

# Logging

(Writing in progress)
