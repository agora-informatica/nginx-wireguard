# nginx-wireguard

Despliegue de servicio vnp wireguard

## Instalar dependencias
```bash 
# apt update
# apt install docker.io docker-compose
``` 

## Cloná el repo y hace deploy
```bash 
# git clone https://github.com/agora-informatica/nginx-wireguard
# cd nginx-wireguard
# docker-compose up -d
```

## Conectar desde el móvil
Mostrar qr code
```bash
# docker-compose logs
```
Luego escaneá el código desde la app de wireguard.

## Conectar desde el ordenador
Exportar peers del servidor al escritorio del cliente:
```bash
# scp -r root@[YOUR_SERVER_IP]:wireguard/peer Desktop/
```
Luego importá los archivos desde la app de escritorio de wireguard.
