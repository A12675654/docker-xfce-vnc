# docker-xfce-vnc
# Docker XFCE + VNC + VSCode + Python + SSH (Ubuntu 24.04)

Aquest projecte permet crear una imatge de Docker basada en **Ubuntu 24.04** amb:
- Entorn gràfic XFCE
- Servidor VNC per a connexió remota
- Visual Studio Code
- Entorn de desenvolupament Python
- Servidor SSH

## Requisits

- Docker instal·lat al vostre sistema host
- Client VNC instal·lat

## Passos per crear i executar el contenidor

### 1. Clonar el repositori
git clone https://github.com/yourusername/docker-xfce-vnc.git
cd docker-xfce-vnc

### 2. Crear la imatge
sudo docker build -t xfce-vnc .

### 3. Executar el contenidor
sudo docker run -d --name xfce-vnc-container -p 5901:5901 -p 2222:22 xfce-vnc

