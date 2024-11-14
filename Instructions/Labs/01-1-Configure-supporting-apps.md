---
lab:
  title: 'Laboratório 1.1: Configurar aplicativos de suporte'
---

# Módulo 1: Configurar o Dynamics 365 Sales

## Laboratório prático 1.1: Configurar aplicativos de suporte

## Cenário

Os vendedores da Contoso Coffee relatam que, embora o Dynamics 365 Sales seja muito útil para aumentar a produtividade do vendedor, o aplicativo parece muito isolado em relação ao fluxo diário de trabalho. Eles têm os seguintes requisitos para seu departamento de TI:

-   Os vendedores gostariam de rastrear e gerenciar a correspondência por email relacionada a vendas no CRM.
-   Os vendedores gostariam de armazenar documentos relacionados a vendas (como artigos de conhecimento do produto, pesquisa de clientes e relatórios de tendências de mercado) no CRM. Eles querem poder acessar, compartilhar e gerenciar esses documentos diretamente do aplicativo Sales.
-   Os vendedores gostariam de colaborar com outros departamentos, como estoque, atendimento de pedidos e marketing, à medida que buscam suas oportunidades de vendas. Eles gostariam que esses outros departamentos pudessem colaborar em um registro de cliente em um chat ou canal do Teams.
-   Os vendedores ouviram muito sobre os recursos do Copilot no Dynamics 365 Sales, incluindo resumo de registros, atualização de alterações nos registros, preparação para reuniões e redação de correspondência. Eles querem garantir que os recursos do Copilot sejam ativados em seu ambiente para que possam começar a utilizar a IA no aplicativo para aumentar sua produtividade.

Neste laboratório, ativaremos e configuraremos os recursos que ajudarão nossa organização de CRM a atender aos requisitos desses vendedores.

## Exercício 1: Configurar a integração de email, SharePoint e OneDrive

### Tarefa 1: Configurar a integração de email

1.  Em um navegador da Web, navegue até [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Na navegação no site no lado esquerdo da tela, selecione **Ambientes**.
3.  Selecione o ambiente **Avaliação do Sales** para abri-lo.
4.  Localize e selecione **Configurações** nos comandos listados na parte superior.
5.  Selecione o cabeçalho do email para expandi-lo e selecione **Caixas de correio.**
6.  Abra o registro de caixa de correio do **administrador do MOD**.
7.  Configure a **caixa de correio do administrador do MOD** da seguinte maneira:
    -   **Perfil do Servidor**: Microsoft Exchange Online
    -   **email de Entrada**: Sincronização no Servidor ou E-mail Router
    -   **email de Saída**: Sincronização no Servidor ou E-mail Router
    -   **Compromissos, Contatos e Tarefas**: Sincronização no Servidor
8.  **Salve** suas alterações. Em seguida, clique em **Aprovar email**. (**Observação:** você deve aprovar a caixa de correio antes de enviar e receber emails).
9.  Será perguntado se deseja aprovar o email principal. Selecione **OK**.
10. Clique em **Testar e habilitar caixa de correio**.
11. Na tela pop-up de teste e habilitação, verifique se essa caixa de correio foi configurada anteriormente para sincronizar com outra organização, marcar essa opção sincronizará com essa organização.
12. Selecione **OK**.

**IMPORTANTE:** não saia desta página enquanto os testes estão sendo concluídos. Se você quiser trabalhar na Tarefa 2 enquanto os testes estão sendo concluídos, você pode abrir uma nova guia ou janela do navegador.

## Tarefa 2: Habilitar a integração com o SharePoint baseada em servidor

Nesta tarefa, você habilitará a integração com o SharePoint baseada em servidor para sua organização do Dynamics 365.

1.  Em um navegador da Web, navegue até [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Na navegação no site no lado esquerdo da tela, selecione **Ambientes**.
3.  Abra o ambiente **Avaliação do Sales** que você tem utilizado para abri-lo.
4.  Localize e selecione **Configurações** nos comandos listados na parte superior.
5.  No cabeçalho Integração, selecione **Configurações de gerenciamento de documentos**.
6.  Você deve ver uma opção para **Habilitar a integração com o SharePoint baseada em servidor**. (Se a opção não estiver lá, a integração com o SharePoint já foi habilitada e você pode pular para a etapa onze.)
    -   Se a Integração com o SharePoint não estiver configurada, selecione **Habilitar integração com o SharePoint baseada em servidor**.
7.  Na tela Habilitar integração com o SharePoint baseada em servidor, clique em **Avançar**.
8.  Selecione **Online** para o tipo de implantação, clique no botão **Avançar**.
9.  Insira a URL do site do SharePoint que deseja usar. (Exemplo: https://"nomeEmpresa".sharepoint.com), clique no botão **Avançar**.

    **Observação:***você pode encontrar o URL do SharePoint ao selecionar o ícone do verificador de aplicativos no canto superior esquerdo da tela. (Parece um quadrado 3 x 3.) mantendo pressionada a tecla CTRL e selecionando SharePoint.*

10. Depois que o site for validado, clique no botão **Ativar**.
11. Clique em **Configurações de gerenciamento de documentos**.
12. Selecione as entidades para as quais você deseja que o gerenciamento de documentos seja habilitado, como Clientes potenciais, Contas, Oportunidades e clique em **Avançar**.
    -   **IMPORTANTE:** se você planeja configurar a interação com email no Sales Insights, selecione a Entidade de email.
13. No campo URL do site do SharePoint, insira a URL do site do SharePoint que você usou na tarefa anterior.
14. Clique no botão **Avançar**.
15. Clique no botão **Finalizar** para concluir a configuração.

### Tarefa 3: Configurar a integração com o OneDrive for Business

Nesta tarefa, você configurará a integração do OneDrie para sua organização do Dynamics CRM. (A partir da publicação deste curso, as configurações de gerenciamento de documentos não estavam disponíveis no centro de administração do Power Platform. Você precisará configurar a integração com o OneDrive for Business na área de configurações clássica do Dynamics 365).

1.  Em um navegador da Web, navegue até [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Na navegação no site no lado esquerdo da tela, selecione **Ambientes**.
3.  Abra o ambiente **Avaliação do Sales** que você tem utilizado para abri-lo.
4.  Localize e selecione **Configurações** nos comandos listados na parte superior.
5.  No cabeçalho Integração, selecione **Configurações de gerenciamento de documentos**.
6.  Clique no ícone **Habilitar OneDrive for Business**.
7.  Marque a caixa de seleção **Habilitar OneDrive for Business** e, em seguida, selecione **OK**.
8.  Depois que a tela for atualizada, clique em **Configurações da pasta do OneDrive for Business**.
9.  Aceite o nome da pasta padrão ou digite um nome de sua escolha e clique em **OK**.

## Exercício 2: Configurar o Teams e o Copilot

### Tarefa 1: Configurar a integração com o Teams

1.  Se necessário, abra o aplicativo Hub de Vendas.
2.  Usando a navegação à esquerda, selecione a área **Vendas** (parte inferior esquerda da tela).
3.  No menu exibido, selecione **Configurações do Aplicativo**.
4.  Em Configurações gerais de grupo, selecione **Chat e colaboração**.
5.  Defina **Ativar a vinculação de registros do Dynamics 365 a canais do Microsoft Teams** como **Sim**.
6.  Defina **Ativar integração avançada com o Microsoft Teams** como **Sim**. (Pode ser necessário selecionar sua conta de administrador do MOD. Se forem solicitadas permissões, selecione **Aceitar**).
7.  Em **Ativar chats do Microsoft Teams no Dynamics 365**, selecione **Ativar para todos os aplicativos do Dynamics 365**.
8.  Selecione o botão **Salvar**.  
    **IMPORTANTE:** pode levar vários minutos para que as alterações sejam salvas.

### Tarefa 2: Configurar o Copilot

1.  Certifique-se de estar na área **Configurações do aplicativo**.
2.  Em Configurações gerais de grupo, selecione **Copilot**.
3.  Marque a caixa de seleção ao lado de **Experimente nossos recursos de visualização mais recentes antes que eles sejam lançados para todos** para ativá-lo.
4.  Em **Recursos do Copilot**, faça as alterações a seguir em **Todos os aplicativos do Dynamics 365 Sales**:
    -   **Chat**: ativado
    -   **Email (versão prévia):** ativado
5.  Selecione o botão **Salvar**.

