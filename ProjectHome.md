# Overview #

This game has a lobby where players can choose their opponents and send invitations. Once another play accepts the invitation, they can play the game together.

This project uses [Apache MINA](http://mina.apache.org/) as the network layer library and [Spring rich client](http://spring-rich-c.sourceforge.net/1.1.0/index.html) as the UI library.

This project is based on the sample project I created for  my article about Apache MINA 2 in Chinese.

Below is a screen-shot of the project.

![http://farm5.static.flickr.com/4093/4783655498_b7f89dda4c.jpg](http://farm5.static.flickr.com/4093/4783655498_b7f89dda4c.jpg)

# Usage #
Download TetrisMina-0.1.0-jar-with-dependencies.jar first, then use the following command to start the server and clients.

Start the server:
```
    java -cp ./TetrisMina-0.1.0-jar-with-dependencies.jar tetrismina.server.ServerMain
```

Start the client:
```
    java -cp ./TetrisMina-0.1.0-jar-with-dependencies.jar tetrismina.client.ClientMain
```

By default, the server is running on port 9190. The client connects to localhost.

# For developers #
This is a [Maven](http://maven.apache.org/) project and you'd better install Maven plug-in for Eclipse to build and debug this project easily.

Please note, the dependency **xswingx** 0.2.0 is not available on Maven repositories. You need to download it from http://code.google.com/p/xswingx/ and install it to your local Maven repository. Refer to [this page](http://jira.springframework.org/browse/RCP-590) for more details.

To test the project, start the server and two clients on the same machine.

# Note #
This project is used to demonstrate some key ideas of Apache MINA and it still has some problems when playing the game.