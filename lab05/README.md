# Aluno

- 216741: George Gigilas Junior

## Tarefa de Cypher sobre Marcadores e Taxonomia

## Tarefa 1

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, sem considerar as categorias subordinadas.

### Resolução

```cypher
match (c:Categoria {id:"Serviços"})
match (m:Marcador)-[:Pertence]->(c)
return m
```

## Tarefa 2

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, considerando as categorias subordinadas.

### Resolução

```cypher
MATCH (a)-[*0..]->(b)
MATCH (m:Marcador)-[:Pertence]->(a)
WHERE
  a:Categoria
  AND b:Categoria
  AND b.id = 'Serviços'
RETURN m
```
