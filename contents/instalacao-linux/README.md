# Instalação do PostgreSQL no Linux

A instalação do PostgreSQL no Linux é bem simples.

## Debian, Ubuntu, Linux Mint e derivados

Execute este comando em um terminal:

``sudo apt-get install postgresql``

## Arch e Manjaro

Execute este comando em um terminal:

``sudo pacman -S postgresql``

# Fedora 

Adicione o repositório ao seu sistema:

``sudo dnf install https://download.postgresql.org/pub/repos/yum/reporpms/F-31-x86_64/pgdg-fedora-repo-latest.noarch.rpm``

Instale o PostgreSQL no seu sistema:

``sudo dnf install postgresql11-server postgresql11``

Confirme a instalação:

``rpm -qi postgresql11-server``

Inialize o PostgreSQL:

```
sudo /usr/pgsql-11/bin/postgresql-11-setup initdb
sudo systemctl start postgresql-11
sudo systemctl enable postgresql-11
```

----

Pronto! o PostgreSQL foi instaldo no seu sistema!