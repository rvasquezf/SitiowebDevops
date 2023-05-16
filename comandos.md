## Los alias
```
https://gist.github.com/MiguelAngelRamos/cfb604f23ae02d804cacb1e1d41f2f59
```

## Comandos para crear una llave ssh

1. Creamos la llave
```shell
ssh-keygen -t rsa -b 4096 -C "tu_email@gmail.com"
```
2. Comprobamos que existan llaves 
```shell
ls -al ~/.ssh 
```
3. Evaluar el servidor SSH ver si esta funcionando.
```shell
eval $(ssh-agent -s)
```
4. Agregamos la llave privada a nuestro servidor

```shell
ssh-add ~/.ssh/id_rsa
```
5. Copiar nuestra llave publica vamos utilizar editor vi

```shell
vi ~/.ssh/id_rsa.pub 
```


## Comandos Git (Github)

1. `git checkout "nombre_de_la_rama"`: Este comando se utiliza para cambiar de la rama actual a la rama especificada. Si la rama existe, pasarás a trabajar en ella.

2. `git branch "nombre_de_la_rama"`: Crea una nueva rama con el nombre especificado. No te cambia a la nueva rama, solo la crea. Si quieres crear y cambiar a la nueva rama en un solo paso, puedes usar `git checkout -b "nombre_de_la_rama"`.

3. `git clone "url_del_repositorio_remoto"`: Este comando copia un repositorio remoto a tu máquina local. Después de clonar, tendrás una copia local del repositorio con todos los archivos, ramas y commits del repositorio remoto.

4. `git merge "nombre_de_la_rama"`: Este comando fusiona los cambios de la rama especificada en la rama actual. Si hay conflictos entre las dos ramas que Git no puede resolver automáticamente, tendrás que resolverlos manualmente antes de poder completar la fusión.