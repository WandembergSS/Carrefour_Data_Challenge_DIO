# Carrefour_Data_Challenge_DIO

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
Os resultados que apresento a seguir, são da versão mais atualizada do projeto, disponível no branch 'Updates'.
  
  De um total de 2663 tweets pesquisados, resultantes dos contextos e querys de pesquisa utilizados, foi descoberto que a Samsung possui popularidade disparada, com os modelos de smartphone Galaxy S20 e A32 sendo os mais comentados, além dominar com outros modelos, deixando nossa tabela de modelos citados:
  
![image](https://user-images.githubusercontent.com/86700373/135449626-d8a8a7b3-e58d-49e3-99e6-4739caef88d7.png)


Onde os modelos Motorola Edge, Redmi 9A, e Realme 8, também aparecem. Essa lista deve aumentar junto com o banco de dados, mas já deve-se notar um problema com nossas buscas. Os ID's dos contextos utilizados não foram encontrados para todas as empresas resultantes do web scraping, deixando nossa pesquisa tendênciosa, apesar de ter utilizado outros parâmetros. 

  Ainda sobre a popularidade, obtemos resultados não surpreendentes, à exceção da Lenovo e Positivo. A Samsung é seguida por essas duas empresas, onde a Lenovo, provavelmente, deve sua popularidade aos seus notebooks, e acredito que houve um erro na análise de sentimento referente a Positivo. Em seguida, como esperado, temos a Apple, Motorola e Xiomi. Além de percebemos que uma competição acirrada com empresas que cresceram muito no mercado brasileiro, como podemos ver no gráfico:
  
 ![image](https://user-images.githubusercontent.com/86700373/135449698-8239e6a5-61fd-41d6-b2bc-d39521d35bea.png)


Com a Wiko recebendo avaliação negativa.
  E por último, do WordCloud criado com os textos de todos os tweets pesquisados, são confirmadas todas as observações feitas até aqui. Além de podermos ver a menção de outros modelos de smartphone, que não são os que aparecem no primeiro gráfico. Além disso, notamos várias palavras relacionadas a notebooks, o que é esperado, pois muitas das empresas que vimos também fabricam esse produto. Mas deve ser notado que não pesquisamos especificamente por esse produto, nos sinalizando que o mercado de notebooks está tão em alta como o de smartphones. Também podemos notar que muitas das palavras estão ligadas a propaganda, indicando que o Twitter é muito utilizada para isso:
  
  ![image](https://user-images.githubusercontent.com/86700373/135449755-5edd867e-9be4-453b-bdc2-1940d23a04f8.png)

  
  Sobre o que pode ser melhorado, diria que os seguintes aspectos potencializariam enormemente os resultados desse projeto:
  1) Uma conta de desenvolvedor com mais recursos;
  2) Uma ferramenta melhor do que a que criei para a busca dos modelos (IA??);
  3) Uma utilização mais integrada com o banco de dados, pois percebi que os recursos disponibilizados pelo Neo4j são vastos, pretendendo me aprimorar, enquanto continuo a desenvolver esse projeto, e em outros.
 
  Por fim, dou uma autoavalição positiva para o projeto que desenvolvi. Primeiro grande projeto que fiz, comparado com os outros publicados por mim no GitHub. Claro, não é um software pronto para ser utilizado por varejistas, mas sim um instrumento de aprendizagem muito rico, pois aqui pude desenvolver muitas coisas aprendidas no bootcamp Carrefour Data Enginer, e conhecer novas ferramentas. Por isso, agradeço imensamente as empresas envolvidas, Digital Inovation One e Grupo Carrefour, por ter icentivado essa experiência.
  
Obrigado!!
