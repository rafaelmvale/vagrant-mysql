# vagrant-mysql
## Principais comandos

- vagrant up (rodar o vagrant)
- vagrant ssh (entrar no ssh via linha de comando)
- mysql -uroot -p (para acessar o user root dentro da maquina)
- passaword: F&Bb7_T!$RNkgMKn

### Dentro do mysql ("mysql>")
- create database "nomedatabase";

#### Criar senha para acessar o database:

- create user nomedatabase@'%' identified with mysql_native_password by 'senhanova';

#### Dar todos os acessos ao  user
- grant all privileges on nomedatabase.* to nomedatabase@'%';
- ctrl D para sair do ambiente
- entrar no ambiente mysql novamente (mysql -uroot-p )
- use nomedatabase;
- CREATE TABLE nometabela (colunas varchar(50),colunas2 integer, PRIMARY KEY (colunas));
- INSERT INTO nometabela VALUES (colunas, colunas2);
- SELECT * FROM nometabela;
