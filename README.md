# vpn

## Instalacion

Ejecutar

```shell
wget https://git.io/vpn -O openvpn-install.sh && bash openvpn-install.sh
chomd +x openvpn-install.sh
./openvpn-install.sh
```

## Configuracion

Editar

```shell
nano /etc/openvpn/server/server.conf
```

### Subredes

Agregar la siguiente linea en el archivo `/etc/openvpn/server/server.conf`

```shell
client-config-dir /etc/openvpn/server/ccd
```

Crear un archivo `Thelonious` en la ruta `/etc/openvpn/server/ccd` agregar la red o subred segun corresponda. Ejemplo:

```shell
iroute 10.108.0.0 255.255.240.0
```
