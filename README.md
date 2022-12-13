# e-commerce_customer_segmentation-


#### Made by Tiago Araujo

# Descrição

Projeto de segmentação de clientes com algoritmos de clusterização para marketplace.

# 1. Problema de negócio

Um marketplace de variados produtos online tem dificuldade de entender seus clientes e confia que a melhor estratégia para reduzir os custos é mazimizar a retenção de clientes. Para isso, precisa de um modelo que indique, de forma automática, quais são os perfis grupos de clientes. O resultado será repassado ao time de marketing para que sejam elaboradas novas estratégias de retenção

# 2. Estratégia de solução

**Etapa 01. Descrição e limpeza de dados **

Objetivo: 
Processo:

**Etapa 02. Filtragem de dados **

Objetivo: 
Processo:


**Etapa 03. Feature Engineering  **

Objetivo: 
Processo:


**Etapa 04. Análise exploratória **

Objetivo: 
Processo:


**Etapa 05. Preparação de dados e redução de dimensionalidade**

Objetivo: 
Processo:


**Etapa 06. Seleção de algoritmos  **

Objetivo: 
Processo:


**Etapa 07. Treinamento de modelos   **

Objetivo: 
Processo:


**Etapa 08. Análise de clusters **

Objetivo: 
Processo:


# 3. Avaliação dos modelos

Para avaliar os modelos, foi usado a métrica de coeficiente de silhueta, que, calculando as distâncias intra e entre clusters, mostra quão bem eles são formados, indo de -1 a 1.


![image](https://user-images.githubusercontent.com/88745881/207449729-6bd184c4-9d64-4dbb-b1d7-26520115bbb5.png)


# 4. Resultado de Negócio

A melhor performance do modelo, considerando a estratégia do negócio, foi a criação de 8 grupos diferentes:

**Cluster 1:**
* Número de customers: 9% dos clientes
* Recência média: 288 dias
* Média de Produtos comprados: 460 produtos
* Frequência de Produtos comprados: 0.76 produtos/dia
* Receita em média: $242.00 dólares
* Estratégia: enviar cupons de desconto com mais frequência para incentivar a fidelização e a diminuição da recência

**Cluster 2:**
* Número de customers:9% dos clientes
* Recência média: 38 dias
* Média de Produtos comprados: 1102 produtos
* Frequência de Produtos comprados: 0.03 produtos/dia
* Receita em média: $323.00 dólares
* Estratégia: como é um grupo que compra em grande quantidade, mostrar anúncios de produtos semelhantes aos comprados por eles, a fim de incentivar compras mais variadas.

**Cluster 3:**
* Número de customers: 13% dos clientes
* Recência média: 21 dias
* Média de Produtos comprados: 506 produtos
* Frequência de Produtos comprados: 0.76 produtos/dia
* Receita em média: $389.00 dólares
* Estratégia: por economia de recursos, não atuar com esse grupo por enquanto, monitorando o seu comportamento

**Cluster 4:**
* Número de customers: 12% dos clientes
* Recência média: 53 dias
* Média de Produtos comprados: 254 produtos
* Frequência de Produtos comprados: 1 produtos/dia
* Receita em média: $341.00 dólares
* Estratégia: enviar cupons de desconto com mais frequência para incentivar a fidelização e a diminuição da recência


**Cluster 5:**
* Número de customers: 12% dos clientes
* Recência média: 74 dias
* Média de Produtos comprados: 501 produtos
* Frequência de Produtos comprados: 0.5 produtos/dia
* Receita em média: $139.00 dólares
* Estratégia: fazer um teste A/B: dividir esse grupo aleatoriamente em 2, enviando e-mails com produtos mais caros para um e mais baratos para outro. O teste tem o objetivo de ver o efeito na recência e na mudança do ticket médio do cliente.

**Cluster 6:**
* Número de customers: 6% dos clientes
* Recência média: 285 dias
* Média de Produtos comprados: 389 produtos
* Frequência de Produtos comprados: 0.8 produtos/dia
* Receita em média: $405.00 dólares
* Estratégia: enviar cupons de desconto com mais frequência para incentivar a fidelização e a diminuição da recência

**Cluster 7:**
* Número de customers: 23% dos clientes
* Recência média: 11 dias
* Média de Produtos comprados: 2575 produtos
* Frequência de Produtos comprados: 0.04 produtos/dia
* Receita em média: $583.00 dólares
* Estratégia: criar um canal de antendimento especializado para esse grupo, a fim de incentivar a manutenção do comportamento de compra.

**Cluster 8:**
* Número de customers: 14% dos clientes
* Recência média: 235 dias
* Média de Produtos comprados: 230 produtos
* Frequência de Produtos comprados: 0.9 produtos/dia
* Receita em média: $248.00 dólares
* Estratégia: enviar e-mails com produtos mais baratos a fim de estimular a compra mais frequente.


# 5. Conclusão

* Com a separação em clusters o negócio consegue focar as estratégias de marketing e personalizar ofertas
* A clusterização pode ser feita de forma automatizada, à medida em que entram novos clientes e antigos mudam seu perfil

# 6. Próximos passos

* Testar outros algoritmos de redução de dimensionalidade e modelos de clusterização
* Colocar o modelo em produção

