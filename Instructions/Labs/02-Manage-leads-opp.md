---
lab:
  title: 'Laboratório 2.1: Gerenciar clientes potenciais e oportunidades'
---

# Módulo 2: Gerenciar clientes potenciais e oportunidades com o Dynamics 365 Sales

## Laboratório prático 2.1: Gerenciar clientes potenciais e oportunidades

### Cenário
A Contoso Coffee está buscando usar o Dynamics 365 Sales para formalizar seu processo de vendas, bem como resolver uma lista de pendências de clientes potenciais novos importados pela equipe de marketing de feiras e campanhas. Como analista de vendas na Contoso Coffee, você foi solicitado a avaliar e atualizar os registros de clientes potenciais para garantir que a equipe executiva esteja trabalhando com base em um relatório de pipeline preciso na próxima reunião de liderança.

Após a conclusão bem-sucedida deste laboratório, você poderá:
- Criar e atualizar registros de clientes em potencial
- Qualificar e desqualificar clientes potenciais
- Reativar registros de clientes potenciais

### Exercício 1 – Gerenciar clientes

#### Tarefa 1 – Criar clientes potenciais
Nesta tarefa, você criará três clientes potenciais, um sem informações da empresa e dois com informações da empresa.
1. Vá para o aplicativo Hub de Vendas do Dynamics 365. Verifique se você está na área Vendas, usando o menu suspenso inferior esquerdo.
2. Usando a barra de navegação à esquerda, selecione **Clientes potenciais** no grupo Vendas.
3. No painel Itens de trabalho, selecione **Grade somente leitura** para alterar o tipo de exibição.
4. No menu exibido, selecione o botão **+ Novo**.
5. Digite *Cliente potencial de máquina de café sem empresa * no tópico, *Jane* no nome e *Doe* no sobrenome.
6. Aceite a sugestão de **Gerente de refeitório** que foi preenchida no campo Cargo.
7. Selecione o botão **Salvar**. Na barra de comandos na parte superior, selecione **+ Novo** novamente.
8. Digite *Cliente potencial de máquina de café com empresa* no Tópico, *Jon* no Nome, *Doe* no Sobrenome, *Doe Inc.* na Empresa e clique em **Salvar.**
9. Na barra de comandos, pressione o botão **+ Novo** mais uma vez.
10. Digite *Outro cliente potencial de máquina de café* no Tópico, *Jack* no Nome, *Rogers* no Sobrenome, *Test Coffee Shop, Inc.* na Empresa e clique em **Salvar.**

### Exercício 2 – Qualificações de clientes potenciais
Neste exercício, você qualificará/desqualificará clientes potenciais e verá quais registros serão criados quando um cliente potencial passar pelo processo de qualificação.

#### Tarefa 1 – Qualificar o cliente potencial da máquina de café sem dados da empresa
1. Vá para o aplicativo Hub de Vendas.
2. Selecionar **Clientes potenciais.**
3. No painel Itens de Trabalho, clique no botão **Grade somente leitura**.
4. Localize **Cliente pootencial de máquina de café sem empresa** e selecione-o.
5. Clique em **Qualificar** no menu superior.
6. O cliente potencial será qualificado em um novo registro de oportunidade.
   - **OBSERVAÇÃO:** se a nova oportunidade não for aberta automaticamente, selecione Oportunidades no menu à esquerda para exibir todas as oportunidades abertas. Em seguida, abra a oportunidade Cliente potencial de máquina de café sem empresa.
7. Localize o campo Contato. Você verá que Jane Doe agora é um registro de contato no aplicativo e agora você pode abrí-lo.
8. Localize o campo Conta (no cabeçalho do registro da oportunidade). Observe que o campo estará vazio.
9. Clique em **Save** (Salvar).

#### Tarefa 2 – Qualificar o Cliente potencial de máquina de café com empresa
1. Vá para o aplicativo Hub de Vendas.
2. Selecionar **Clientes potenciais**.
3. Localize Cliente potencial de máquina de café com empresa e abra-o.
4. Clique em **Qualificar** no menu superior.
5. O cliente potencial será qualificado como o cliente potencial anterior e você será levado para o registro de oportunidade recém-criado do cliente potencial qualificado.
6. Localize o campo Contato. Você verá que Jon Doe agora é um registro de contato.
7. Localize o campo Conta. Você verá que a Doe, Inc. agora é um registro de conta.

#### Tarefa 3 – Desqualificar um cliente potencial
1. Se necessário, vá para o aplicativo Hub de Vendas.
2. Selecionar **Clientes potenciais.**
3. Localize Outro cliente potencial de máquina de café e abra-o.
4. Clique em **Desqualificar** (talvez seja necessário selecionar o botão de reticências verticais para que a opção seja exibida).
5. Em seguida, no menu apresentado, selecione **Não está mais interessado**.
6. O cliente potencial será desqualificado, o status mudará para "Não está mais interessado" e o registro se tornará somente leitura.

#### Tarefa 4 – Reativar um cliente potencial
1. Se necessário, vá para o aplicativo Hub de Vendas.
2. Na navegação no site, no grupo Vendas, selecione **Clientes potenciais.**
3. O cliente potencial que você desqualificou não está mais na visualização Meus clientes potenciais abertos. Selecione a seta para baixo ao lado de Meus Clientes Potenciais Abertos e altere a exibição para **Clientes Potenciais Fechados.**
4. Localize Outro cliente potencial de máquina de café e abra-o.
5. Clique em **Reativar cliente potencial**.
6. O cliente potencial será reativado, o status mudará de volta para Novo e o registro se tornará editável.

### Exercício 3 – Trabalhar com oportunidades
Neste exercício, você percorrerá o processo de trabalhar com uma oportunidade por meio do processo de vendas.

#### Tarefa 1 – Gerenciar o cliente potencial de máquina de café com empresa
1. Se necessário, vá para o aplicativo Hub de Vendas.
2. Usando a barra de navegação à esquerda, selecione **Oportunidades** no grupo Vendas.
3. Localize e abra a oportunidade **Cliente potencial de máquina de café com empresa**.
4. No painel de Oportunidade exibido, selecione o **botão Ir para Principal **(localizado ao lado do botão X (Fechar)).
5. Preencha o registro de oportunidade da seguinte maneira:
   - Valor do orçamento: US$ 17.000
   - Período de Compra: este trimestre
   - Processo de compra: comissão
   - Descrição: buscando atualizar suas máquinas de café atuais em vários locais.
6. Expanda o cabeçalho do registro na parte superior e conclua da seguinte maneira:
   - Data estimada de fechamento: insira a data de amanhã.
   - Data estimada: US$ 16,500
7. No controle de Linha do tempo, selecione **+** (adicionar um registro de linha do tempo).
8. No menu exibido, selecione **Telefonema**.
9. Preencha o telefonema da seguinte maneira:
   - Assunto: chamada inicial para Jon.
   - Conclusão: insira a data de hoje às 16h30.
10. Selecione o botão **Salvar e Fechar **.
11. Com a Oportunidade aberta, selecione **Estágio de desenvolvimento** no fluxo de processo empresarial de Cliente Potencial para Oportunidade. Preencha o seguinte:
   - Necessidade do cliente: buscando atualizar suas máquinas de café em vários locais.
   - Solução proposta: recomendar várias máquinas AirPot Duo.
   - Identificar os stakeholders: concluído
   - Identificar os concorrentes: concluído
12. Selecione o botão **Próximo estágio**.
13. No estágio Propor, defina todos os campos como **Concluído.**
14. Selecione o botão **Próximo estágio**.
15. Selecione qualquer lugar fora do estágio do processo empresarial para fechá-lo.
16. Na seção Assistente, em Notificações, selecione o item **Telefonema** que você criou anteriormente para abri-lo.
17. Selecione **Concluir**. (Observe que o item desaparece de suas notificações.)
18. No processo de vendas Cliente Potencial para Oportunidade, selecione o **estágio de Fechamento**.
19. Marque todos os itens no estágio Fechamento como **Concluídos.**
20. Selecione o botão **Concluir**.
21. Na barra de comandos na parte superior, selecione o botão **Fechar como ganho**.
22. Na tela Fechar oportunidade, selecione o botão **OK**.

Parabéns, você criou e gerenciou com sucesso clientes potenciais e oportunidades no Dynamics 365 Sales.
