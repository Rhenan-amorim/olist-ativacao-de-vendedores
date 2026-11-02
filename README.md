# Quais origens de lead trouxeram lojistas que chegaram à primeira venda na Olist?

[Abrir o estudo de caso de Rhenan Amorim](https://rhenan-amorim.github.io/olist-ativacao-de-vendedores/)

Analisei o funil de aquisição de lojistas da Olist para decidir quando a equipe comercial deveria oferecer ajuda após o fechamento. Entre 548 vendedores com 90 dias completos de acompanhamento, 228 registraram ao menos uma venda observada nesse período.

| Origem | Fechamentos elegíveis | Lojistas com venda observada | Ativação |
|---|---:|---:|---:|
| Busca paga | 121 | 66 | 54,5% |
| Busca orgânica | 175 | 65 | 37,1% |

A diferença entre as taxas foi de 3,2 pontos percentuais aos 30 dias e chegou a 13,1 pontos aos 60 dias. Eu testaria um contato adicional no dia 30 com quem ainda não vendeu. Nesse momento, 243 vendedores das duas origens seriam elegíveis para o contato. O estudo apresenta o desenho do teste e a consulta SQL usada para calcular a ativação.

Cruzei leads e negócios por `mql_id` e vinculei os vendedores aos pedidos por `seller_id`. Cada lojista conta uma única vez. A primeira venda é a primeira compra aprovada observada na amostra após o fechamento. As taxas descrevem o histórico dessas origens e o efeito do atendimento proposto continua em aberto.

Fontes públicas anonimizadas da Olist: [funil comercial](https://www.kaggle.com/datasets/olistbr/marketing-funnel-olist) e [pedidos de e-commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).
