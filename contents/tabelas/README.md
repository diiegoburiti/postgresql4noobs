# Criando Tabelas no PostgreSQL

Para criar uma table em PostgreSQL iremos usar o comando `CREATE TABLE` dessa maneira:

```sql
CREATE TABLE usuarios (
    id SERIAL PRIMARY KEY,
    nome varchar(20),
    sobrenome varchar(20),
    idade int
);
```

Foi usado `SERIAL` ao invés de `int`, pois `SERIAL` a cada vez que inserimos um dado automaticamente o id é incrementado, assim não precisamos ficar pesquisando qual foi o ultimo id inserido e somar mais um, pois o PostgreSQL já irá fazer isso.

Para criarmos a tabela, podemos inserir o nome, depois `(`, todos os campos e seus tipos primitivos, separando com uma vírgula, e fechando com um `);`.

Criamos um id, sendo `SERIAL`. nome sendo um `varchar(20)`, assim o nome terá no máximo 20 caracteres, a mesma coisa com o sobrenome e a idade sendo `int`, representando um número inteiro.