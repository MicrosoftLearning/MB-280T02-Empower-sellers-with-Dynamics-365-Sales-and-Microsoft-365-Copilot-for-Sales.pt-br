---
lab:
  title: 'Laboratório 6.1: Configurar um painel'
---

# Módulo 6: Analisar dados do Dynamics 365 Sales

## Laboratório prático 6.1: Configurar um painel

### Cenário
Os gerentes de vendas da Contoso Coffee querem monitorar o sucesso da equipe de vendas com mais eficiência, especialmente em relação a oportunidades fechadas. Um gerente de vendas solicitou um painel pessoal que fornecerá uma visão geral das oportunidades fechadas recentemente e das ações de seus vendedores em relação a elas. Além disso, eles prefeririam que esse painel fosse o painel padrão quando abrissem a seção Painéis do aplicativo.

Após a conclusão deste laboratório, você saberá:
- Criar painéis pessoais
- Adicionar componentes aos painéis

## Exercício 1 – Configurar um painel 
### Tarefa 1 – Criar um painel
1. Certifique-se de estar na área Vendas do aplicativo, caso ainda não esteja. Use o menu suspenso inferior à esquerda para alterar a área para **Vendas** se precisar alternar.
2. No grupo Meu Trabalho, selecione **Painéis** no menu de navegação à esquerda.
3. Por padrão, o Painel Social de Atividades de Vendas será exibido. Sinta-se à vontade para explorar os vários componentes. Além disso, você pode usar o ícone suspenso <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> ao lado do título do painel para explorar os outros painéis do sistema.
4. Quando estiver tudo pronto para criar o painel, clique em **+ Novo** e em **Painel do Dynamics 365.**
5. Explore os vários layouts de painel. Nesta tarefa, criaremos um Painel regular de duas colunas. Quando estiver tudo pronto, selecione-o na lista e selecione **Criar.**

### Tarefa 2 – Adicionar componentes
1. O designer do painel será aberto em uma nova janela. (Se o novo painel não abrir em uma nova janela, certifique-se de que o bloqueador de pop-ups esteja desativado.) O designer pode levar um minuto para carregar.
2. Na caixa de texto Nome, digite *Painel do Gerente de Vendas*.
3. Vamos adicionar um componente à seção superior esquerda. Os gerentes de vendas estão solicitando uma maneira fácil de ver a quantidade de receita ganha versus perdida de oportunidades. Eles querem essas informações em uma exibição gráfica. Para fazer isso, adicionaremos um gráfico clicando no ícone **Inserir gráfico** no meio da seção superior esquerda.
4. Selecione os seguintes detalhes do seu gráfico:
   - Tipo de Registro: Oportunidade
   - Exibição: Oportunidades fechadas
   - Gráfico: Negócios ganhos vs. negócios perdidos
   - Selecione **Adicionar**.
5. Seu gráfico aparecerá na seção superior esquerda.
6. Em seguida, vamos adicionar um componente à seção superior direita. Os gerentes de vendas estão solicitando uma maneira de visualizar de forma fácil as oportunidades fechadas recentemente para que possam verificar com os vendedores as lições aprendidas. Eles querem que a exibição inclua oportunidades ganhas e perdidas, mas apenas oportunidades fechadas no ano fiscal atual. Clique no ícone **Inserir lista** para a seção superior direita.
7. Selecione os seguintes detalhes da sua lista:
   - Tipo de Registro: Oportunidades
   - Exibição: Oportunidades fechadas no ano fiscal atual
   - Clique em **Adicionar**.

### Tarefa 3 – Salvar e editar o painel
1. Clique em **Salvar** e **Fechar**. A janela será fechada e você retornará ao formulário Painéis, onde seu novo painel será exibido.
2. Na barra de comandos, clique em **Definir como Padrão**. Esse painel agora será seu painel padrão quando você navegar para a seção Painéis.
3. No menu superior, clique em **Editar**. Você retornará ao designer do painel em outra nova janela. Adicione mais dois componentes abaixo do gráfico. Os componentes selecionados devem resolver os seguintes requisitos de negócios solicitados pelos gerentes de vendas:
   - Os gerentes de vendas querem ter uma noção de como os vendedores individuais estão se saindo com base na receita de oportunidades fechadas deles. Eles querem um gráfico que mostre os nomes dos vendedores e a receita total de oportunidades fechadas de cada um.
   - Os gerentes de vendas querem monitorar as tarefas diárias dos vendedores em sua equipe. Eles querem ver uma lista que mostre as atividades das equipes de vendas.
