---
tags:
  - conceito
  - datascience
  - pandas
  - python
aliases: []
fonte: "[[Análise de Padrões no Brasileirão]]"
---

# Filtrando e criando novos data frames no Pandas

### Resumo (Com minhas palavras)
Alguma vez durante a sua análise você precisou filtrar dados? Ou filtrar os dados para criar um novo data frame?

Bom, se você não passou por isso, tenho certeza que irá passar porque é um processo muito comum durante nossas análises já que quase sempre estamos filtrando ou isolando valores. Se você usa o Pandas no seu dia a dia, esse processo é ainda mais simples e rápido.

Vem comigo que eu vou te mostrar o código e explicar a sintaxe dele. 

Existem duas maneiras de filtrar um valor no pandas:

V1:
```python
filtro_campeoes = df["place"] == 1

df_campeoes = df[filtro_campeoes].reset_index(drop=True)
```
V2:
```python
df_campeoes = df[df["place"] == 1].reset_index(drop=True)
```

A diferença primordial entre o V1 e V2 é só a praticidade, no V1 você cria uma lógica ou regra de negócio e replica ela em diferentes data frames, no V2 a replicação em diferentes data frames é um pouquinho mais chatinha e se torna até mais complicada se você precisar mudar algo porque vai precisar mudar de 1 por 1.

Basicamente, nessa filtragem nos estamos passando pro nosso *df* que queremos apenas os valores que dentro do nosso *df* possuem na coluna "place" o número 1, esse é o nosso filtro. Mas, o que significa o resto do código? 

Bom, o `df_campeoes =`é bem lógica, estamos filtrando o *df* e atribuindo o retorno a uma nova variável e essa variável agora é um novo data frame, a parte do `reset_index(drop=True)` é mais gosto pessoal, quando criamos um novo data frame a partir de dados filtrados de outro, ele traz os indexes do antigo data frame, então se em um data frame o valor que você filtrou for o de index 4233, no novo data frame o valor não muda, ele vai permanecer igual e só muda se você forçar o pandas a fazer isso, a parte do `drop=True`é porque na chamada padrão da função, depois de resetar os indexes, ele cria uma nova coluna com os indexes antigos, esse parâmetro com o **True** diz para ele não fazer isso.

Assim, com essas simples e fáceis linhas de comandos você pode filtrar e criar novos data frames no pandas.

### Insights / Conexões
- Isso me lembra de 
- Pode ser aplicado em 

### Referências / Links Relacionados
- Relacionado: [[Como criar novas colunas dentro de um data frame do Pandas]], [[03 - Introdução a DSA (O que envolve DS)]]