# Universidade de Montana

<img src="https://github.com/jefferson-datascience/project_university_montana/blob/main/logo_university.jpg" alt="logo" style="zoom:80%;" />

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

# 2. Estratégia de Solução

Para esse tipo de problema, utilizamos a seguinte estratégia.

**Etapa 00. Carregamento dos Dados:** Organização dos dados disponibilizados pela Universidade.

**Etapa 01. Escolha do Teste:** Escolher do Tipo de Teste que será utilizado para resolver o problema de negócio.

**Etapa 02. Design de Experimento:** Formulação das hipóteses nula, hipótese alternativa, definição da métrica e definição de parâmetros do teste como nível de confiança, nível de significância e poder estatístico.

**Etapa 03. Preparação e Coleta dos Dados de Amostragem:** Preparação dos Dados em uma tabela de contigência.

**Etapa 04. Teste de Hipótese:** Cálculo do p-valor e validação das hipóteses nula e alternativa e realização do Post-Hoc

**Etapa 05. Conclusão do Teste:** Apresentação de relatório com a conclusão do Teste.

# 3. Conclusão do Teste

Nesse experimento estatístico, nós utilizamos o teste chi-quadrado de independência para saber se os títulos do botões tem um impacto na taxa de cliques. Assumindo as hipóteses abaixo: 

**Hipótese Nula:** Não há uma relação entre os títulos dos botões e os cliques.

**Hipótese Alternativa:** Há uma relação entre os títulos dos botões e os cliques.

e com um p_valor de 2.0959498129984567e-09, concluímos que algum(ns) dos título tem um impacto na quantidade de cliques. Uma vez obtida essa informação, nós realizamos o teste post-hoc com o teste chi-quadrado para saber como era a relação dois a dois dos botões em relação ao botão "Interact". No fim, concluímos que os botões "Connect", "Help" e "Service" possuem um impacto na taxa de cliques comparados com o botão "Interact". Para ver o desenvolvimento do experimento, basta clicar nesse link: **[Experimento 01](https://github.com/jefferson-datascience/project_university_montana/blob/main/Project%20University%20Montana/notebooks/teste_relacao_titulos_cliques.ipynb)**

# 4. Próximos Passos

Como o objetivo do teste é dizer se existe alguma variação do botão que impacte de forma positiva as taxas de cliques, foi necessário realizar um novo experimento estatístico. Clique aqui para ver o planejamento do **[Experimento 02]()**.
