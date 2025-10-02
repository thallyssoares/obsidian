---
tags:
  - conceito
  - datascience
  - python
  - pandas
aliases: []
fonte: "[[Análise de Padrões no Brasileirão]]"
---

# Aplicando funções elaboradas no Pandas

### Resumo (Com minhas palavras)
Alguma vez você já precisou criar funções mais elaboradas ou aplicar regras de negócio mais complexas para os seus data frames só que ficou preso nas limitações do pandas?

Bom, tenho uma boa noticia para você, seus problemas acabaram!

Existe uma função no pandas que foi pensada justamente para esses casos onde não existe algo na biblioteca que resolva o que você precisa, essa função é o `.apply()`. 

Essa função pode ser usada de duas maneiras essenciais, aplicando funções que você cria por fora ou aplicando funções dentro dela como se fosse um `for`. Abaixo o exemplo de cada aplicação:

Função externa
```python
df_rebaixado1 = df.groupby("season", group_keys=False).apply(identificar_rebaixados)
```

Função interna
```python
maisRebaixadoPorPosicao = df_rebaixado.groupby("place")["team"].apply(lambda x: x.value_counts().idxmax())
```

No exemplo da função externa, eu tinha um problema nos meus dados em que "season" especificas possuíam tipos de critérios diferentes do padrão, assim, criei uma função externa que receberia os meus dados do data frame e analisaria a partir de cada "season" qual era e qual regra aplicar.

Já no exemplo da função interna, meu problema poderia ser resolvido com funções do próprio Pandas mas exigiam uma abordagem mais complexa. Basicamente, eu precisava pegar qual time ficou mais vezes em determinada posição e isso exigia um aninhamento de funções que só foi possível com o `apply()`. Como eu disse, ele parece o `for`porque criamos uma variável temporária e que só será usada nessa situação e nela que fazemos as aplicações.

Viu só, criar funções mais elaboradas é extremamente simples no Pandas e seus usos são infinitos.

### Insights / Conexões
- Isso me lembra de
- Pode ser aplicado em

### Referências / Links Relacionados
- Relacionado: [[Como criar novas colunas dentro de um data frame do Pandas]], [[Filtrando e criando novos data frames no Pandas]], [[03 - Introdução a DSA (O que envolve DS)]]