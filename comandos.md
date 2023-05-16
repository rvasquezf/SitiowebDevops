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