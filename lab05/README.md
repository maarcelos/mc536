# Modelo para Apresentação do Lab05 - Marcadores e Taxonomia em Cypher

Estrutura de pastas:

~~~
├── README.md  <- arquivo apresentando a tarefa
~~~

# Aluno
* `240765`: `Marcelo Salles Previti`

## Tarefa de Cypher sobre Marcadores e Taxonomia

## Tarefa 1

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, sem considerar as categorias subordinadas.

### Resolução
~~~cypher
MATCH(m:Marcador)
MATCH(n:Categoria)
WHERE n.id = "Serviços" and (m)-[:Pertence]->(n)
RETURN m
~~~

## Tarefa 2

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, considerando as categorias subordinadas.

### Resolução
~~~cypher
MATCH (m:Marcador)
MATCH(c:Categoria)
MATCH(n:Categoria {id:"Serviços"})
WHERE (c)-[*]->(n) or c.id = "Serviços" and (m)-[:Pertence]->(c)
RETURN  m
~~~
