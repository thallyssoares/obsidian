---
tags:
  - captura
  - python
  - pandas
  - datascience
disciplina: Pandas
fonte: Inspiração [https://www.youtube.com/watch?v=7yB5GTUHAFc]
data: 01.10.2025
---

# Tópico: Análise de Padrões no Brasileirão

---
### Resumo Imediato
Após ver o vídeo que está citado na fonte, me inspirei para criar um mini projeto de análise de dados com os dados do brasileirão.

Nesse projeto, minha ideia foi simular como se eu fosse um analista de um time recém promovido para a série A e o time tivesse me solicitado uma análise dos últimos para entender padrões entre os campeões e os rebaixados transformando isso em recomendações para o técnico e time de scout na montagem do elenco.

Nesse trabalho usei principalmente o pandas, aplicando suas formulas principais e criando algumas regras de negócios usando funções a parte(Isso eu acabei pedindo ao gemini).

Como próximos passos, penso que posso usar a biblioteca do Seaborn para criar gráficos que casem com as minhas análises do pandas e além de olhar outras métricas, como nesse caso do brasileirão que eu poderia ter olhado para o saldo de gols entre campeões e rebaixados, poderia ter olhado a média de pontos e a taxa de vitória do 16 colocado para ter uma noção mais exata dos valores que salvaram algum time.

De qualquer maneira, proveitoso o projeto e me ajudou a validar meus aprendizados bem como descobrir coisas novas.


Abaixo segue a task e hipóteses formuladas com suas respostas:
```
Você é um analista de dados de um time recém promovido para a série e precisa analisar as informações sobre os últimos 22 campeões do brasileirão e sobre os times que foram rebaixados nesses respectivos anos, afim de encontrar padrões entre os melhores times e entre os piores times para trazer insights para a comissão técnica e para o time de scout sobre que time precisamos montar.

  

Hipoteses

- O time que tem o melhor ataque é o time campeão? e os times de pior ataque são os times rebaixados?: Olhando em média, os times de melhor ataque são os campeões onde 75% dos times campeões apresentou uma média de gols médios entre 1.3 e 1.8 gols. Enquanto isso, os times rebaixados entregam uma média de 1 gol em média por jogo e 75% varia entre 0.4 e 1.17 gols. Mostrando que, de fato, times campeões possuem melhores médias de gols por jogo e times rebaixados as piores.

- O time de melhor defesa é o campeão? e os times de pior defesa são os rebaixados?: Na defesa a situação é a mesma do ataque. Enquanto times campeões mostram uma média abaixo de 1 gol por jogo, times rebaixados entregam 1.5 gols por jogo. Quando olhamos pra distribuição dos dados, 75% dos times campeões tem entre 0.5 e 0.99 gols cedidos em média já os rebaixados tem entre 0.97 e 1.75, o que demonstra que um time não rebaixado é um time que acima de tudo, não toma muitos gols.

- Existe uma taxa de vitória média para não ser rebaixado?: Sim, em média os times rebaixados fizeram uma taxa de 22% com a grande maioria fazendo menos do que 26% de taxa de vitória, sendo assim, para uma margem segura, 31% de taxa de vitória assegura o não rebaixamento do time.

- Recomendações: Com isso, como analista do time, minha recomendação é focarmos em construir um time defensivamente solido e que não toma muitos gols, não precisamos de uma ataque extremamente poderoso com 1.5 gols de média por jogo, precisamos apenas que esse time não tome muitos gols por jogo e que faça os necessários. Assim, conseguiremos buscar uma taxa de vitórias de 31%, necessária para nos livrar do rebaixamento, resultados acima disso já serão suficientes para nos entregar vagas em competições internacionais.

```
### Fila de Síntese Imediata ⚡
- [ ] [[Como criar novas colunas dentro de um data frame do Pandas]]
- [ ] [[Filtrando e criando novos data frames no Pandas]]
- [ ] [[Aplicando funções elaboradas no Pandas]]