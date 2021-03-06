  Esse projeto foi desenvolvido com o intuito de participar do Data Challenge, promovido pelo Banco Carrefour e pela Digital Inovation One, com entrega até 26 de setembro de 2021. 
Para este desafio, deve-se criar uma aplicação para monitorar as top trendings do Twitter e seu devido volume. Pelo caráter personalizado dos assuntos mais discutidos na rede 
social, disponibilizados aos seus usuários pela própria plataforma, foi tomada a liberdade de filtro dos top trendings sobre smartphones e seus fabricantes.

   Antes de tudo, foi realizado um webscraping, de modelos de smartphones dos últimos 3 anos. O projeto foi feito primariamente em python, consumindo a API do Twitter e armazenando os dados relevantes em um banco de dado do tipo grafos, o neo4j. Onde os gráficos de visualização desses dados foram criados no próprio script. O código foi desenvolvido para consulta diaria, sendo estruturado de forma a pesquisar tweets das últimas 24h.

 Basicamente, a ideia é fornecer três tipos diferentes de vizualização:
1) Trends em WordCloud relativo a todos os tweets armazenados até o momento; 
2) Gráfico de popularidade das empresas.
3) Modelos de smartphones mais comentados.

 Onde a análise de popularidade de cada empresa foi esimada a partir da soma dos índices de popularidade de cada tweet, indo de -1 à 1. Assim, a popularidade deve crescer com a frequência de citações, bem como com os próprios resultados das análises de sentimento. Com isso, desejo fornecer ferramentas que auxiliem profissionais do varejo na tomada de decisões que impulsionem vendas. Como, por exemplo, na decisão de quais produtos comprar, de campanhas de promoção, e em saber quais produtos mantêm-se populares, além das tendências no geral.

 
Obs: Devido a taxa limitada de solicitações de pesquisa no API do Twitter, não pude coletar muitos dados até a data de entrega do projeto. Os arquivos do projeto, continuam no repositório, enquanto updates do projeto estão no branch 'Updates'.





## Resultados:
  
  De um total de 2876 tweets pesquisados, resultantes dos contextos e querys de pesquisa utilizados, foi descoberto que a Samsung possui popularidade disparada, com os modelos de smartphone Galaxy S20 e A32 sendo os mais comentados, além dominar com outros modelos, deixando nossa tabela de modelos citados:
  
![image](https://user-images.githubusercontent.com/86700373/135713622-c7c021c6-e7e7-46a0-af9b-3c90f5bc81ba.png)




Onde os modelos Motorola Edge, Redmi 9A, e Realme 8, também aparecem. Essa lista deve aumentar junto com o banco de dados, mas já deve-se notar um problema com nossas buscas. Os ID's dos contextos utilizados não foram encontrados para todas as empresas resultantes do web scraping, deixando nossa pesquisa tendênciosa, apesar de ter utilizado outros parâmetros. 

  Ainda sobre a popularidade, obtemos resultados não surpreendentes, à exceção da Lenovo e Positivo. A Samsung é seguida por essas duas empresas, onde a Lenovo, provavelmente, deve sua popularidade aos seus notebooks, e acredito que houve um erro na análise de sentimento referente a Positivo. Em seguida, como esperado, temos a Apple, Motorola e Xiomi. Além de percebemos que uma competição acirrada com empresas que cresceram muito no mercado brasileiro, como podemos ver no gráfico:
  
![image](https://user-images.githubusercontent.com/86700373/135713648-a7ca2d01-fee4-4b53-9c76-5c06ab729eb0.png)



Com a Wiko recebendo avaliação negativa.
  E por último, do WordCloud criado com os textos de todos os tweets pesquisados, são confirmadas todas as observações feitas até aqui. Além de podermos ver a menção de outros modelos de smartphone, que não são os que aparecem no primeiro gráfico. Além disso, notamos várias palavras relacionadas a notebooks, o que é esperado, pois muitas das empresas que vimos também fabricam esse produto. Mas deve ser notado que não pesquisamos especificamente por esse produto, nos sinalizando que o mercado de notebooks está tão em alta como o de smartphones. Também podemos notar que muitas das palavras estão ligadas a propaganda, indicando que o Twitter é muito utilizada para isso:
  
![image](https://user-images.githubusercontent.com/86700373/135713676-e1f46e2d-d1bf-4dcd-8540-3343fde3b4db.png)


  
  Sobre o que pode ser melhorado, diria que os seguintes aspectos potencializariam enormemente os resultados desse projeto:
  1) Uma conta de desenvolvedor com mais recursos;
  2) Uma ferramenta melhor do que a que criei para a busca dos modelos (IA??);
  3) Uma utilização mais integrada com o banco de dados, pois percebi que os recursos disponibilizados pelo Neo4j são vastos, pretendendo me aprimorar, enquanto continuo a desenvolver esse projeto, e em outros.
 
  
