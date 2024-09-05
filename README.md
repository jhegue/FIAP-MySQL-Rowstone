# MySQL Rowstore

# Definição

Row-oriented database é o tipo mais tradicional de banco de dados onde os atributos (colunas) de um registro são organizadas sistematicamente em linhas e armazenadas juntos.

## Setup
Cria o clone do repositório:
```
git clone git clone https://github.com/jhegue/FIAP-MySQL-Rowstone.git
```

>### Importante!
>Os comando deste laboratório presumem que estamos no diretório raiz do projeto.

## Configurações
No diretório `server/mysql/etc/` encontra-se um arquivo `my.cnf` que contém os parâmetros de configuração do MySQL.<br>
Embora não seja escopo deste laboratório o entendimento detalhado do MySQL, recomendo o estudo do arquivo `my.cnf`.

```
ls -latr server/mysql/etc/my.cnf
```

Output:
```
user@brubeck:~/labs/mysql8$ ls -latr server/mysql/etc/my.cnf
-rw-r--r-- 1 user user 581 sep 16 14:46 server/mysql/etc/my.cnf
```

## Docker
Será utilizado o MySQL em um container baseado em *Docker*.<br>
Na raiz do projeto está disponível um arquivo `compose.yaml` que contém os parâmetros de inicialização do container Docker.<br>
