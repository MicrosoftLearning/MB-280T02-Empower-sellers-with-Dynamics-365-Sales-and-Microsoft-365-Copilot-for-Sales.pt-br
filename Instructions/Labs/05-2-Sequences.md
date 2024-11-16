---
lab:
  title: 'Laboratório 5.2: Criar uma sequência'
---

# Módulo 5: Trabalhar com o Dynamics 365 Sales Insights e o Acelerador de vendas 

## Laboratório prático 5.2: Criar uma sequência

### Cenário
Os vendedores da Contoso Coffee sugerem que as vendas poderiam ser melhoradas se as "melhores práticas" organizacionais fossem mais fáceis de seguir. Após análise, os gerentes de vendas da Contoso determinaram uma sequência ideal de eventos de vendas para os vendedores. Eles querem aplicar as práticas recomendadas configurando uma série de atividades consecutivas para os vendedores seguirem enquanto qualificam clientes potenciais. Você quer garantir que seja o mais fácil possível para os vendedores seguirem durante o dia. Você determinou que uma sequência é a melhor maneira de fazer isso.

Após a conclusão deste laboratório, você saberá:

-   Criar um segmento
-   Criar uma sequência
-   Definir atividades de sequência
-   Ativar e conectar sequências aos registros

## Exercício 1: Criar e anexar sequências a registros

### Tarefa 1: Habilitar o Acelerador de vendas

1.  No grupo Insights de vendas, selecione **Configurações globais.**
2.  No subgrupo Acelerador de vendas, clique na guia **Sequências**.
3.  Será solicitado que você configure o espaço de trabalho para poder usar Sequências. Clique no botão **Configurar espaço de trabalho**.
4.  Clique no botão **Configuração rápida**.
5.  Na seção Tipo de registro e formulário, clique em **+ Adicionar tipo de registro**. Clique em **Oportunidades**.
6.  Para o formulário padrão para cada tipo de registro, configure da seguinte maneira:
    -   Clientes potenciais: Insights de vendas
    -   Oportunidades: Insights de vendas
7.  Selecione o botão **Publicar**.
    -   Observação: pode levar alguns minutos para que as alterações sejam aplicadas.

### Tarefa 2: Criar um segmento

1.  Se você ainda não tiver feito isso, altere a área para **Configurações de Insights de vendas.**
2.  No grupo Insights de vendas, selecione **Configurações globais.**
3.  No subgrupo Acelerador de vendas, clique na guia **Atribuição de trabalho**.
4.  Certifique-se de que o **Tipo de registro** esteja definido como **Clientes potenciais** e clique no botão **Novo segmento**.
5.  No campo **Nome**, insira o texto **Clientes potenciais de feiras de negócios** e clique no botão **Avançar**.
6.  Na guia **Definição de segmento**, clique no botão **Adicionar**.
7.  No menu exibido, selecione **Adicionar linha**.
8.  Configure a condição da seguinte maneira:
    1.  **Fonte de clientes potenciais** – **Igual** – **Feira**
9.  Selecione **Simular resultados**.

    Você verá uma tela de simulação de membro do segmento que incluirá todos os clientes potenciais que atendem aos seus critérios.

10. Feche a janela de **Simulação de membro do segmento**.
11. Selecione o botão **Salvar**.
12. Clique no botão **Ativar**.

## Exercício 2: Criar e anexar sequências a registros

### Tarefa 1: Criar nova sequência

1.  Se você ainda não tiver feito isso, altere a área para **Configurações de Insights de vendas.**
2.  No grupo Insights de vendas, selecione **Configurações globais.**
3.  No subgrupo Acelerador de vendas, clique na guia **Sequências**.
4.  Se necessário, selecione **Habilitar** na notificação para habilitar o fluxo de trabalho para que as sequências funcionem corretamente.
5.  Na guia Sequências, clique em **+ Nova sequência**.
6.  Você tem a opção de criar uma sequência a partir de vários modelos comuns. Você pode explorar os modelos disponíveis. Quando estiver tudo pronto, clique em **Começar do zero**.
7.  Em seguida, você atribuirá um nome, uma descrição e escolherá o tipo de tabela para a qual a sequência estará disponível. Na caixa de texto Nome da Sequência, digite o nome da sequência: *Sequência de Acompanhamento da Feira de negócios.*
8.  Na caixa de texto Descrição, insira a descrição da sequência: "Esta é uma sequência de teste para a Test Coffee. Essa sequência será usada para acompanhar clientes em potencial após as feiras."
9.  Em Tipo de registro, selecione **Cliente potencial** (se ainda não estiver selecionado).
10. Clique em **Avançar**.

### Tarefa 2: Escolher a primeira atividade que o vendedor deverá realizar

Escolha o que os vendedores deverão fazer em primeiro lugar. Isso pode ser enviar um email, fazer uma ligação ou adicionar uma tarefa própria. Em nosso exemplo, começaremos com um email.

1.  Abaixo do bloco Início da sequência, clique no botão **+** para adicionar uma ação ou outro elemento.
2.  Clique em **Enviar um email.**
3.  Em Título, insira: *Email de introdução*.
4.  Em Descrição, você tem a opção de inserir uma descrição: *Apresentar o cliente potencial à equipe de vendas.*
5.  Se modelos de email (modelos específicos de tabela ou globais) estiverem disponíveis em sua organização, você poderá escolher um modelo de email. Nesse caso, vamos supor que o vendedor escreverá seu próprio email de apresentação.
6.  Clique no **X** para fechar o painel Atividade.
7.  Na barra de comandos da sequência, clique em **Salvar**.

### Tarefa 3: Adicionar outras atividades para seu vendedor executar

Adicione atividades adicionais para seus vendedores realizarem seguinte uma ordem – por exemplo, o vendedor precisa fazer a primeira atividade primeiro, depois a segunda e a terceira e assim por diante.

1.  Clique no botão **+**.
2.  Escolha a próxima atividade para o vendedor realizar, pode ser enviar um email, fazer uma ligação ou adicionar uma tarefa própria. Selecione **Definir tempo de espera** para definir um intervalo de tempo entre as atividades. Em nosso exemplo, adicionaremos um intervalo de tempo de 1 hora.
3.  Clique em Save (Salvar).
4.  Clique no botão **+**.
5.  Selecione **Telefonema**.
6.  No Título, insira *Chamada de acompanhamento.* (Você pode optar por adicionar uma descrição, se desejar.)
7.  Selecione **Salvar** na barra de comandos.

### Tarefa 4: Ativar a sequência

Para disponibilizar a sequência para os vendedores usarem, ative-a.

1.  Selecione **Ativar** na barra de comandos.
2.  Selecione **Eu entendo** e, em seguida, **Ativar** no pop-up.
3.  Sua sequência agora terá uma barra verde na parte superior informando que a sequência foi ativada.

### Tarefa 5: Conectar uma sequência a um segmento

1.  Verifique se você está na área de **configurações de Insights de Vendas**.
2.  Na navegação à esquerda, selecione **Sequências**.
3.  Abra a sequência de **Acompanhamento da feira** que você criou anteriormente.
4.  Selecione a guia **Clientes potenciais conectados**.
5.  Selecionar **+ Conectar segmentos**
6.  Localize e selecione o segmento **Clientes potenciais de feiras** que você criou anteriormente.
7.  Selecione **Conectar**.

### Tarefa 6: Conectar a sequência ao registro (Do registro)

1.  Altere a área para a área de **Vendas** usando o menu suspenso inferior à esquerda.
2.  Selecione **Clientes potenciais** no menu de navegação do site.
3.  Selecione um dos clientes potenciais que você criou anteriormente.
4.  Na barra de comandos, clique na **seta para baixo** ao lado de Sequências. No menu exibido, clique em **Conectar sequência** na barra de comandos.
5.  Selecione a sequência criada anteriormente e selecione **Conectar.**
6.  Uma mensagem de confirmação aparecerá na parte inferior da página e a sequência será conectada ao registro de cliente potencial selecionado.
7.  Se for solicitado que você atribua um vendedor, clique no botão **Atribuir**. Agora, os vendedores que têm acesso ao registro de cliente potencial podem ver as atividades conectadas a ele.
8.  Atualize a página – você verá as tarefas que criou na seção **A seguir**.

