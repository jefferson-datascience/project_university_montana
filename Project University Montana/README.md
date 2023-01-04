# Experimento Estatístico 02 - Universidade de Montana

<img src="[https://github.com/jefferson-datascience/project_eletronic_house/blob/main/images/logo_eletronic_house.jpg](https://github.com/jefferson-datascience/project_university_montana/blob/main/logo_university.jpg)" alt="logo" style="zoom:80%;" />



# 1. Problema a Ser Resolvido.

Sabendo que os botões "Connect", "Help" e "Service" impactam a taxa de cliques quando comparados ao botão "Interact", o nosso problema agora é saber quais desses botões é melhor que o interact e, por fim, responder a seguinte questão: 
 
1. Alguma das conversões é realmente melhor do que a atual? Qual seria o nome da variação?


 ## Planejamento da Solução?
 
**Qual vai ser a solução para o problema?** A solução para esse problema é uma aplicação de teste A/B sobre os seguintes botões: ("Connect", "Interact"), ("Help", "Interact") e ("Service", "Interact")
 
**Qual vai ser o produto final?** O produto final será um relatório com as questões de negócios respondida. 


# 2. Estratégia de Solução

Para esse tipo de problema, utilizamos a seguinte estratégia.

**Etapa 00. Carregamento dos Dados:** Organização dos dados disponibilizados pela Universidade.

**Etapa 01. Escolha do Teste:** Escolher do Tipo de Teste que será utilizado para resolver o problema de negócio.

**Etapa 02. Design de Experimento:** Formulação das hipóteses nula, hipótese alternativa, definição da métrica e definição de parâmetros do teste como nível de confiança, nível de significância e poder estatístico, cálculo do effect size e determinação do tamanho da mostra para o teste ter o mínimo de validade.

**Etapa 03. Preparação e Coleta dos Dados de Amostragem:** Separação dos dados em seus respectivos grupos.

**Etapa 04. Teste de Hipótese:** Cálculo do p-valor de cada grupo e realização das validações das hipóteses nula e alternativa sobre cada Grupo.

**Etapa 05. Conclusão do Teste:** Apresentação de relatório com a conclusão do Teste e resposta da questão de negócio.

# 3. Conclusão do Teste

Nesse teste o objetivo foi verificar a diferença na proporção de taxas de cliques entre os botões em seus respectivos grupos e verificar qual possuia uma melhor efetividade. Concluímos que os botões "Connect", "Help" e "Services" obtem um melhor desempenho o botão "Interact" sendo que o botão com melhor efetividade é o "Connect". Para acessar o experimento estatístico e os códigos desenvolvidos, basta clicar no link: **[Experimento 02](https://github.com/jefferson-datascience/project_university_montana/blob/main/Project%20University%20Montana/notebooks/teste_botoes_efetividade.ipynb)**

# 4. Respondedo a Questão de Negócio

**1. Alguma das conversões é realmente melhor do que a atual? Qual seria o nome da variação?**

A resposta é sim! O Botão "Connect" é a opção.

