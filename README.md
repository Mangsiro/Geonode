# Geonode
instalasi GeoNode 3.2.x berbasis shell script untuk Ubuntu 20.04
Ubuntu 20.04 (Ubuntu, WSL2), Ubuntu 18.04 (WSL2)

# Unduh Instalasi Geonode 3.2
```
wget https://raw.githubusercontent.com/Mangsiro/Geonode/main/install-geonode-dockerimage.sh
wget https://raw.githubusercontent.com/Mangsiro/Geonode/main/install-master-geonode.sh
```

# Install Docker image 
```
chmod +x install-geonode*
./install-geonode-dockerimage.sh
```
# Check Docker Image Terpasang
dilakuakan docker image sudah berhasil terpasang
```
docker run -it hello-world
```
# Install Master Geonode 3.2
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

Default user name: admin

Default password: admin

>untuk mengakhiri geonode 
```
cd /opt/geonode
docker-compose stop
```
