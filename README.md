# Sw



Master:

 docker pull nginx
   -  docker images
   -  mkdir demo
   -  cd demo/
   -  nano index.html
   -  cd
   - ls
   - mkdir tinku
    -cd tinku/
     -  nano index.html
   - nano Dockerfile
     -  cd
  

   - cd tinku/
     -  docker build -t poojax/prac1doc .
   - docker images
-  docker login -u poojax -p pqrDOC@11.11
   -  docker push poojax/prac1doc

   - docker swarm init
   -  docker swarm init --advertise-addr 192.168.56.104
     -  docker node ls
   - docker service create --name web -p 80:80 -d poojax/prac1doc
     -  docker images
   - docker service scale web=3
     -  docker ps


Worker :

 sudo usermod iacsd -aG docker
   - docker swarm join --token SWMTKN-1-0stskslatoliveiig5thaw32132eu465u19wzraq4ywcjijr87-8i30efejeuxneez74ts5rk72i 192.168.56.104:2377
- docker ps
