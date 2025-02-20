git clone https://github.com/bruxx70/test-craftech.git
cd test-craftech

# build 
docker-compose up --build -d

# verifico esta corriendo correctamente
docker ps

#Por motivos de tiempos simplemente lo generé con docker compose, la idea era construir la solucion que corra en kubernetes al menos generearlo con minikube para simular el cluster.