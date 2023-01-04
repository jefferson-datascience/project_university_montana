# Universidade de Montana

<img src="https://github.com/jefferson-datascience/project_eletronic_house/blob/main/images/logo_eletronic_house.jpg" alt="logo" style="zoom:80%;" />

O objetivo deste projeto é realizar um teste A/B/n para verificar a efetividade de cliques de alguns botões de uma página.

O contexto de negócio é fictício. Todavia, o planejamento, execução, desenvolvimento e implementação da solução seguem todos os passos de um projeto real.

Os dados do problema de negócio estão disponíveis no meu drive: https://drive.google.com/file/d/1oUJLeAgSaUI7CA-0F14KG0FzXEim7pSe/view

#### This project was made by Jefferson Henrique Candido.

# 1. Problema de Negócio.

A Universidade de Montana, nos Estados Unidos, possui vários serviços de apoio ao aluno, incluido a biblioteca.

A biblioteca da universidade oferece vários serviços para os estudantes como alocação de salas de estudo, livros, computadores, discussões em grupo, webnários e etc. Todos esses serviços e vários outros ficam disponíveis dentro da página web da prórpia biblioteca e os alunos podem acessá-las para agendar algum dos serviços disponíveis.

A página possui um banner da universidade, uma barra de busca, três principais categorias de acesso e uma barra lateral direita que exibi as últimas notícias.

Durante o período de 3 de Abril de 2013 até 10 de Abril de 2013, a página "home" da biblioteca recebeu 10.819 visitantes. Ao analisar os dados de acesso da página, o time de TI da Universidade percebeu uma grande diferença entre os acessos das categorias das páginas. A taxa de click da "Find" foi de 35%, "Request" foi de 6% e "Interact foi de 2%.

Olhando para as taxas de click, o time de TI se perguntou o motivo da conversão da categoria "Interact" estar tão baixa.

Uma das hipóteses do time de TI foi de que o nome "Interact" está confundindo os alunos, pois não deixa claro o propósito daquela categoria. Assim, novos nomes foram propostos para substituir o nome da atual categoria: "Connect", "Lean", "Help" e "Service".

Com as variações do nome da categoria, um teste A/B/n precisa ser definido para validar qual das variações deixa a categoria mais compreensível e atraente para os estudantes, com a expectatica de aumentar a taxa de clicks nessa categoria.

Assim, um teste A/B/n foi realizado durante 3 semanas, entre os dias 29 de Maio de 2013 e 18 de Junho de 2013. O experimento foi desenhado para garantir que um usuário pudesse acessar qualquer uma das variações com a mesma probabilidade.

Assim, o nosso objetivo é responder a seguinte questão:
 
1. Alguma das conversões é realmente melhor do que a atual? Qual seria o nome da variação?


 ## Planejamento da Solução?
 
**Qual vai ser a solução para o problema?** A solução para esse problema é uma aplicação de teste A/B/n sobre os dados disponibilizados pela Universidade.
 
**Qual vai ser o produto final?** O produto final será um relatório com as questões de negócios respondida. 


# 3. Estratégia de Solução

**Etapa 00. Carregamento dos Dados:** Carregar os dados, Visualização Geral dos Dados.

**Etapa 01. Escolha do Teste:** Escolher do Tipo de Teste que será utilizado para resolver o problema de negócio.

**Etapa 02. Design de Experimento:** Formulação das hipóteses nula, hipótese alternativa e definição da métrica e determinação do tamanho da amostra.

**Etapa 03. Preparação e Coleta dos Dados de Amostragem:** Verificação de dados nulos e duplicidade de flags e homogeneidade dos dados. Em  seguida, separação dos grupos controle e tratamento, coleta das amostragem e cálculo das taxas de conversões.

**Etapa 04. Teste de Hipótese:** Determinação da melhor inferência, cálculo do p-valor e validação das hipóteses nula e alternativa.

**Etapa 05. Conclusão do Teste:** Apresentar o relatório respondendo a questão de negócio.

# 4. Conclusão do Teste

Não conseguimos seguir com o experimento na Espanha, Grã-Bretanha, Turquia, Alemanha, França, Austrália e Canadá, pois faltam dados para realizar a amostra. Tanto para os dados do site quanto para os dados do App. Conseguimos das prosseguimento com os dados somente do Brasil, México e Estado Unidos.

Para os Dados do Site, foi formulada as seguintes hipóteses:

**Hipótese Nula:** O preechimento automático e o preenchimento manual possuem a mesma média de quantidade gasta pelo site.

**Hipótese Alternativa:** O preechimento automático e o preenchimento manual possuem média de compras finalizadas diferentes pelo site.

Nos dados do site do Brasil, México e Estados Unidos falhamos em rejeitar a hipótese nula, onde os p-valores são, respectivamente, 0.5904, 0.992 e 0.5490 com um nível de significância de 0.05. 

Para os Dados do App, foi formulada as seguintes hipóteses:

**Hipótese Nula:** O preechimento automático e o preenchimento manual possuem a mesma média de quantidade gasta pelo app.

**Hipótese Alternativa:** O preechimento automático e o preenchimento manual possuem média de compras finalizadas diferentes pelo app.

Nos dados do site do Brasil, México e Estados Unidos também falhamos em rejeitar a hipótese nula, onde os p-valores são, respectivamente, 0.2209, 0.284 e  0.3616 com um nível de significância de 0.05. 


# 5. Respondendo as Questões de Negócio

Como não há dados suficiente da Espanha, Grã-Bretanha, Turquia, Alemanha, França, Austrália e Canadá para realizar a amostra, informamos ao Head de Designers que não há dados suficientes para para realizar a inferência sobre esses países e que pode ser adota a seguinte estratégia:

1. Realizar uma maior coleta de dados. 
    
    - Nessa situação, é importante ter em mente qual vai ser o custo desta coleta de mais amostras para que se tenha uma quantidade mínima para observar se há um lift de 8% na média de gastos dos clientes.

Para os dados do Brasil, México e Estados Unidos, não houve diferença na média de gastos utilizando o formulário automático ou manual, tanto pelo site quanto pelo app.

Nesse contexto, podemos tomar a seguinte atitude com o Head de Designers.

1. Informar ao Head de Designers para solicitar a sua equipe uma melhoria no design do formulário automático.

    - Nessa situação, com uma melhoria no formulário, é esperado que se observe um efeito maior na quantidade média de gastos, isto é, um maior lift esperado em relação ao formulário manual.
    
    
2. Informar ao Head de Designers para solicitar uma nova amostragem.
    
    - Nessa situação, é primordial saber os custos e o tempo necessário para se realizar uma nova coleta de dados, pois com essas informações saberemos se com o lift esperado do formulário automático valerá a pena realizar essa nova coleta de dados.

# 7. Próximos Passos

  Os próximos passos desse projeto é levantar os custos de todo o processo de produção da página até o processo de coleta de amostra para saber o quanto que tem que ser o mínimo de lift dessa nova página para que se pague os custos de todo esse processo e além disso se obtenha o faturamento esperado.


**Clique aqui para acessar o código e todo o desenvolvimento do projeto:** https://github.com/jefferson-datascience/project_eletronic_house/blob/main/conversao_formulario_pagamento/notebooks/6.0%20-%20jhc.conversao_formulario_pagamento.ipynb
