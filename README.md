# Sw



Master:

 docker pull nginx
   62  docker images
   63  mkdir demo
   64  cd demo/
   65  nano index.html
   66  cd
   67  ls
   68  mkdir tinku
   69  cd tinku/
   70  nano index.html
   71  nano Dockerfile
   72  cd
  

   77  cd tinku/
   78  docker build -t poojax/prac1doc .
   79  docker images
   80  docker login -u poojax -p pqrDOC@11.11
   81  docker push poojax/prac1doc

   83  docker swarm init
   84  docker swarm init --advertise-addr 192.168.56.104
   85  docker node ls
   86  docker service create --name web -p 80:80 -d poojax/prac1doc
   87  docker images
   88  docker service scale web=3
   89  docker ps


Worker :

 sudo usermod iacsd -aG docker
   57  docker swarm join --token SWMTKN-1-0stskslatoliveiig5thaw32132eu465u19wzraq4ywcjijr87-8i30efejeuxneez74ts5rk72i 192.168.56.104:2377
   58  docker ps
