# docker-dosbox

Run [DOSBox](https://www.dosbox.com/) in a docker container. I run it on my NAS.

1. Add your game archives or folders (you can get games e.g. from https://dosgames.com/)
2. Run `docker build -t dosbox .`
3. Start with `docker run -p 8080:8080 dosbox` or if you use a volume `docker run -p 8080:8080 -v /local/folder/with/games:/root/dos dosbox`
4. Connect with a browser to your docker host e.g. http://localhost:8080



=======================================================================

##IN PRACTICAL SCENARIO


CONTAINER ID   IMAGE             COMMAND                CREATED          STATUS          PORTS                                       NAMES
e700638f9f73   mydosbox:latest   "/app/entrypoint.sh"   24 minutes ago   Up 24 minutes   0.0.0.0:8080->8080/tcp, :::8080->8080/tcp   hardcore_tharp




Links:  https://dosgames.com/
https://dosgames.com/game/fury-of-the-furries/


https://earthly.dev/blog/dos-gaming-in-docker/

https://www.retrogames.cz/play_1627-N64.php

https://www.retrogames.cz/download_Genesis.php?id=595&ROMfile=http://www.retrogames.cz/Genesis/Pocahontas.zip


git hub:    https://github.com/schneidexe/docker-dosbox


mobigames: https://www.mobygames.com/

==============================================






 5  docker ps
 
    6  git clone https://github.com/schneidexe/docker-dosbox.git
    7  ls
    8  cd docker-dosbox
    9  ls
    
   10  cat Dockerfile 
   
   11  ls
   
   12  docker  build -t mydosbox .
   
   13  ls
   
   14  mkdir  games
   
   15  ls
   
   16  cd games
   
   17  pwd
   
   18  docker run -d -v /root/docker-dosbox/games:/root/games/ -p 8080:8080 mydosbox:latest 
   
   19  docker ps 
   
   20  ls
   
   21  pwd
   
   22  docker ps 
   
===============


   15  git clone https://github.com/anirudhadak2/kucl2023.git
   
   16  ls
   
   17  cd kucl2023
   
   18  ls
   
   19  ls -la
   
   20  ls
   
   21  unzip DOSBOX_ALADDIN.ZIP
   
   22  ls
   
   23  pwd
   
   24  ls
   25  cd 
   
   26  ls
   
   27  cd /root/docker-dosbox/games
   
   28  ls

   29  cd ..
   
   30  ls
   
   31  docker build -t mydosbox .
   
   32  ls
   
   33  docker run -d -v /root/docker-dosbox/games:/root/games/ -p 8080:8080 mydosbox:latest 
   
   34  ls
   
   35  docker ps
   
   36  ls
   
   37  cd games
   
   38  ls
   
   39  pwd
   
   40  cd 
   
   41  ls
   
   42  cd kucl2023
   
   43  ls
   
   44  cp DOSBOX_ALADDIN.ZIP /root/docker-dosbox/games
   
   45  ls
   
   46  cd /root/docker-dosbox/games
   
   47  ls
   
   48  unzip 
   
   49  unzip /root/docker-dosbox/games
   
   50  ls
   
   51  unzip DOSBOX_ALADDIN.ZIP


==============================================
then access the container on  8080 port no.  and then 

select ==> 

Directory listing for /
app/
core/
include/
utils/
vendor/
vnc.html
vnc_auto.html@
vnc_lite.html

==>  Select  
vnc_auto.html@ 

the dosbox  terminal will open 
in terminal 
z:>  
z:> mount  c:  /root/games      ==> mount to the directoy where the container dir is mounted
z:> c:
c:> dir 
c:> aladdin   (game name)  the game will run 

==========================================================



