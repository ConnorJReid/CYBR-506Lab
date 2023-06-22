# CYBR-506Lab
this is for the final docker project for cyber 506

Set UP instructions:
1 pull the files off github
2 enter your terminal and traverse to the directory of the downloaded file. 
3 run the command: docker build -t lab6 
4 run the command: docker run -d --name my-radius-server -p 1812:1812/udp -p 1813:1813/udp
5 enter into the container's terminal via the docker app and enter the command: radtest connor 1130 localhost 0 testing123
6 create a second instance of the running docker container under a different name. 
    run the command: docker run -d --name my-radius-server -p 5000:5000/udp -p 5000:5000/udp
7 enter into NEWLY CREATED container's terminal via the docker app and enter the command: radtest connor 1130 127.0.0.1:1813 1130

