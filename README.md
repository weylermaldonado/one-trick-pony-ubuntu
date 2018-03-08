# Ubuntu tricks

## Agregar una aplicación .AppImage a escritorio
Creamos un archivo .desktop en el siguiete directorio
```bash
$ cd ~/.local/share/applications
```
```bash
$ touch app.desktop
```
Luego lo abrimos y escribimos lo siguiente
```bash
$ nano app.desktop
```
```nano
[Desktop Entry]
Type=Application
Name=Minecraft
Comment=Minecraft
Icon=/home/bram/Applications/Minecraft/icon.png
Exec=/home/bram/Applications/Minecraft/minecraft
Terminal=true
Categories=Minecraft;game
```
Reiniciamos nautilus si es necesario
```bash
$ nautilus -q
```
o
```bash
$ killall nautilus
```

## Crear alias  temporar

```bash
$ alias current_command='custom_command'
```
## Crear alias permanente
```bash
$ sudo nano .bashrc
```
Al final del documento, creamos algo como
```bash
$ alias proyecto="cd /home/usuario/Documentos/Web"
```

## Detener instancia de MySQL
```bash
$ sudo service mysql stop
```
