# Selecionando Dados

Para selecionar dados em bancos de dados PostgreSQL usamos o ``SELECT``, que é um comando que seleciona dados que uma tabela. Podemos modificar como usaremos este comando, mas a forma mais fácil de usar ele é esta:

``SELECT * FROM usuarios;``

Este SELECT irá retornar TODOS os dados de todos os usuários da tabela, para criarmos uma query (consulta) usando o SELECT, colocamos * no lugar que especifica quais campos da tabela iremos buscar, pois * é um caractere coringa que representa qualquer coisa, e no caso, seria todos os campos, e depois o FROM seguido do nome da tabela, que é usuários.

Para pegarmos apenas, por exemplo, o nome e o sobrenome, podemos substituir o * por ``nome, sobrenome``, que assim, iremos pegar pegar apenas o nome e o sobrenome de todos os registros da tabela.

``SELECT nome, sobrenome FROM usuarios;``

E para pegarmos apenas um registro específico da tabela, que tem o nome "Pedro" podemos usar ``WHERE``, que com ele, podemos pegar apenas um registro onde uma certa condição é verdadeira, segue o exemplo:

``SELECT nome, sobrenome FROM usuarios WHERE nome = 'Pedro';``

Há muitas possibilidades há mais que podem ser feitas usando o SELECT, junto com o JOIN por exemplo, mas por este tutorial ser mais exuto, não será apresentado este tipo de conteúdo, que você pode procurar por conta própria.