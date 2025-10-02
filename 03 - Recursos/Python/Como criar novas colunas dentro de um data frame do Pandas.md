---
tags:
  - conceito
  - datascience
  - python
  - pandas
aliases: []
fonte: "[[Análise de Padrões no Brasileirão]]"
---

# Como criar novas colunas dentro de um data frame do Pandas

### Resumo (Com minhas palavras)
Nem sempre a base de dados que estamos trabalhando para a nossa análise possui todas as colunas com as métricas que precisamos, mas muita das vezes ela tem duas colunas que formam a métrica que queremos ver. 

Com isso, surge a dúvida, como criar novas colunas dentro do nosso data frame para usarmos em nossa análise?

Para a sua felicidade isso é muito simples no pandas, vou mostrar um exemplo de código e explico melhor sobre ele: 
```python
df["percentual_vitorias"] = df["won"] / df["played"] * 100
```

Como podemos ver, o processo de criação de novas colunas usa uma sintaxe parecida com a que usamos para referenciar colunas existentes do nosso **data frame**. Usamos `df["nome_da_coluna"] = a lógica da coluna` nesse caso do exemplo estamos criando a coluna "percentual_vitorias" e estamos dizendo pro pandas que essa coluna é o resultado da divisão da coluna `df["won"]`pela coluna `df["played"]`multiplicado por 100 para ficar mais visual a porcentagem. 

Com isso, o pandas vai percorrer linha por linha do nosso data frame e criar essa coluna fazendo essa operação com os dados respectivos de cada linha.

Pronto, simples assim você criou uma nova coluna no pandas.


### Insights / Conexões
- Isso me lembra de .
- Pode ser aplicado em .

### Referências / Links Relacionados
- Relacionado: [[Filtrando e criando novos data frames no Pandas]], [[03 - Introdução a DSA (O que envolve DS)]]