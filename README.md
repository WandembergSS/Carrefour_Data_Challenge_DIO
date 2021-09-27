# Carrefour_Data_Challenge_DIO

  Esse projeto foi desenvolvido com o intuito de participar do Data Challenge, promovido pelo Banco Carrefour e pela Digital Inovation One, com entrega até 26 de setembro de 2021. 
Para este desafio, deve-se criar uma aplicação para monitorar as top trendings do Twitter e seu devido volume. Pelo caráter personalizado dos assuntos mais discutidos na rede 
social, disponibilizados aos seus usuários pela própria plataforma, foi tomada a liberdade de filtro dos top trendings sobre smartphones e suas fabricantes.

   Antes de tudo, foi realizado um webscraping, de modelos de smartphones dos últimos 3 anos. O projeto foi feito primariamente em python, consumindo a API do Twitter e armazenando os dados relevantes em um banco de dado do tipo grafos, o neo4j. Onde os gráficos de visualização desses dados foram criados no próprio script. O código foi desenvolvido para consulta diaria, sendo estruturado de forma a pesquisar tweets das últimas 24h.

 Basicamente, a ideia é fornecer três tipos diferentes de vizualização:
1) Trends em WordCloud relativo a todos os tweets armazenados até o momento; 
2) Gráfico de popularidade das empresas.
3) Modelos de smartphones mais comentados.

Assim, desejo fornecer ferramentas que auxiliem profissionais do varejo na tomada de decisões que impulsionem vendas. Como, por exemplo, na decisão de quais produtos comprar,
de campanhas de promoção, e em saber quais produtos mantêm-se populares, além das tendências no geral.

 
Obs: Devido a taxa limitada de solicitações de pesquisa no API do Twitter, não pude coletar muitos dados até a data de entrega do projeto. Os arquivos do projeto, continuam no repositório, enquanto updates do projeto estão no branch 'Updates'.
