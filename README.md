# Geonode
instalasi GeoNode 3.2.x Instalasi script berbasis untuk Ubuntu 20.04
Ubuntu 20.04 (Lubuntu, WSL2), Ubuntu 18.04 (WSL2)

# Unduh Instalasi Geonode 3.2
```
Wget https://raw.githubusercontent.com/Mangsiro/Geonode/main/install-geonode-dockerimage.sh
wget https://raw.githubusercontent.com/Mangsiro/Geonode/main/install-master-geonode.sh
```

# Install Docker image 
```
chmod +x install-geonode*
./install-geonode-dockerimage.sh
```
# Check Docker Image Terpasang
pastikan docker image sudah berhasil terpasang
```
docker run -it hello-world
```
# Install master geonode
```
./install-master-geonode.sh
```
# Check Geonode Terpasang
```
cd /opt/geonode
docker logs -f django4geonode
```

# Memulai Geonode 
> untuk memulai geonode 
```
  cd /opt/geonode
  docker-compose start
```
Browse GeoNode instalasi pada search engine (http://localhost)
```
Default user name: admin
Default password: admin
```
# Mengakhiri geonode 
```
  cd /opt/geonode
  docker-compose stop
```

