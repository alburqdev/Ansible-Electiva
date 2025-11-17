# Ansible-Electiva

# Práctica de Automatización con Ansible + Docker

Este repositorio contiene la práctica donde se crean 5 servidores Ubuntu usando Docker y se automatiza la instalación de paquetes y creación de usuarios mediante Ansible.

## 🚀 Contenido
- Dockerfile con instalación de SSH
- docker-compose con 5 servidores Ubuntu
- Inventario Ansible
- Playbooks:
  - Actualización del sistema
  - Creación de usuario itla
  - Creación de carpeta y archivo
  - Instalación de cowsay y htop

## ▶️ Cómo levantar los servidores
```bash
cd docker
docker compose up -d
