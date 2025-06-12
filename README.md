# docker_nginx_proxy_manager

Docker-compose para desplegar un servidor nginx-proxy-manager + dashboard con metricas + modo oscuro + archivo con listado de anti-crawlers.

Testeado con qemu + ubuntu2404 + vagrant

---

### Descripción

El proyecto cuenta con los archivos necesarios para levantar usando docker un servicio [nginx-proxy-manager](https://nginxproxymanager.com/guide/) para pruebas de laboratorio.

### Dependencias

* [Docker](https://docs.docker.com/engine/install/ubuntu/)
* [Docker-Compose](https://docs.docker.com/compose/install/standalone/)
* [Vagrant](https://developer.hashicorp.com/vagrant/install) (opcional)

### Uso
```shell
git clone https://github.com/pgraffigna/docker_nginx_proxy_manager.git
cd docker_nginx_proxy_manager
docker-compose up -d
```

### Extras
* Vagrantfile: Archivo de configuración para desplegar una VM descartable con ubuntu-22.04 con libvirt como hipervisor.
* 98-themepark-npm: dark mode
* block-exploits.conf: anti-crawlers
* env: variables de entorno
