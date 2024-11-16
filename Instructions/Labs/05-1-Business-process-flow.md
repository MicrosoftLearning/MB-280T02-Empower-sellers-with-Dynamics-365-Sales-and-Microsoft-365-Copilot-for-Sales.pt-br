---
lab:
  title: 'Laboratório 5.1: Personalizar um fluxo do processo empresarial'
---

# Módulo 5: Trabalhar com o Dynamics 365 Sales Insights e o Acelerador de vendas 

## Laboratório prático 5.1: Personalizar um fluxo do processo empresarial

## Cenário

A Contoso Coffee quer adicionar algumas etapas extras ao Processo Empresarial de Vendas testado e comprovado. Embora os vendedores tenham tido bons resultados seguindo essa estrutura no passado, eles estão relatando que algumas novas sugestões ajudariam a nutrir clientes potenciais e conseguir contratos de alto valor.

Os vendedores querem adicionar as seguintes etapas ao processo empresarial:

-   Para clientes em potencial de alto valor com um orçamento acima de \$1.000.000, peça ao líder de vendas que entre em contato pessoalmente para confirmar o interesse antes de passar para a qualificação.
-   No estágio de desenvolvimento, certifique-se de que os vendedores estejam acompanhando os pontos problemáticos existentes do cliente para ajudar a identificar possíveis áreas de vendas complementares que podem ter sido perdidas anteriormente.

Neste laboratório, personalizaremos o fluxo do processo empresarial para atender às solicitações de nossos vendedores.

## Exercício 1 – Personalizar o fluxo do processo empresarial

### Tarefa 1: Criar o fluxo do processo empresarial

Nesta tarefa, você criará um novo Fluxo do Processo Empresarial (BPF) a partir do Processo de Vendas de Oportunidade e, em seguida, testará o novo BPF.

1.  Navegue até [https://make.powerapps.com](https://make.powerapps.com/).
2.  Verifique se você está no ambiente **Avaliação de Vendas**.
3.  Selecione **Soluções**.
4.  Na barra de comandos na parte superior, clique no botão **+ Nova solução**.
5.  No campo **Nome de exibição**, insira **Contoso**.
6.  Clique em **+ Novo editor**.
7.  Configure o novo editor da maneira a seguir.
    1.  **Nome de exibição:** Contoso
    2.  **Nome:** Contoso
    3.  **Prefixo:** Contoso
    4.  **Prefixo do valor de escolha:** 10000
8.  Selecione **Salvar**.
9.  Em Editor, selecione o novo editor da **Contoso** que você acabou de criar.
10. Selecione **Criar**.
11. Na **Barra de comandos**, selecione **Adicionar** existente.
12. No menu exibido, selecione **Processo de****automação**\>.
13. Agora, encontraremos o **Processo de Vendas** na lista de processos. (Agora você pode usar a caixa de pesquisa no canto superior direito para pesquisar.) Quando você encontrá-lo, selecione-o.
14. Selecione o botão **Adicionar**.
15. Selecione o **Processo de Vendas** para abri-lo.
16. Uma nova guia abrirá o editor do BPF. (Mantenha a guia antiga com a lista Soluções aberta.) Agora, vamos adicionar as etapas que nossos vendedores estão pedindo.
17. Primeiro, adicionaremos uma condição para verificar o orçamento do cliente e identificar nossos clientes potenciais de alto valor com orçamentos acima de\$1.000.000. Arraste **Condição** da guia **Componentes** e coloque-a entre os estágios **Qualificar** e **Desenvolver**.
18. Selecione a **Condição**, vá para a guia **Propriedades** e insira **Verificar orçamento** em **Nome de exibição**.
19. Em **Regras**, selecione **Valor do Orçamento** em **Campo**.
20. Selecione **Maior ou igual a** em **Operador**.
21. Selecione **Valor** em **Tipo**.
22. Insira **1.000.000** em **Valor** e clique em **Aplicar**.
23. Agora precisamos adicionar um novo estágio para completar a condição. No painel Componentes, adicione um novo Estágio à direita da Condição.
24. Clique na guia **Propriedades**.
25. Insira **Confirmar interesse** em **Nome de exibição**. Escolha **Aplicar**.
26. Clique no botão **Detalhes** do estágio **Confirmar interesse**.
27. Selecione a **Etapa de Dados\# 1 Nova Etapa** dentro do estágio **Confirmar interesse**.
28. Na guia **Propriedades**, abra a lista suspensa em **Campo de dados.** Clique em **Confirmar interesse**. O nome da etapa será atualizado automaticamente.
29. Marque a caixa de seleção **Obrigatório** e clique em **Aplicar**.
30. Em seguida, adicionaremos uma nova etapa para perguntar os pontos problemáticos do cliente no estágio de desenvolvimento, conforme solicitado por nossos vendedores. Selecione o estágio **Desenvolver** e expanda **Detalhes**.
31. No painel Componentes, arraste uma **Etapa de Dados** abaixo da Etapa de Dados \#4.
32. No menu suspenso Campo de dados, selecione **Pontos problemáticos do cliente**. Agora esta será uma etapa sugerida no estágio de desenvolvimento para identificar os pontos problemáticos do cliente. Não marcaremos este campo como obrigatório.
33. Escolha **Aplicar**.
34. Clique em **Validar** para garantir que as alterações feitas sejam válidas e que o BPF funcione conforme o esperado.
35. Se estiver tudo certo, clique em **Atualizar**.
36. Feche a guia com o editor de Fluxo do processo empresarial.
37. De volta à guia anterior, clique em **Concluído** no pop-up na área Solução padrão. No menu superior, selecione **Publicar todas as personalizações.** (Talvez seja necessário excluir a pesquisa de "oportunidade" na caixa de texto no canto superior direito para poder ver esse botão.)
38. Aguarde a **publicação** das personalizações.

### Tarefa 2 – Testar o fluxo do processo empresarial

1.  Volte ao aplicativo Hub de Vendas.
2.  Navegue até a seção **Oportunidades** e clique em **+Novo** para criar uma nova oportunidade. Insira um tópico como **Interesse em novas máquinas**.
3.  Selecione um contato existente para o campo de contato.
4.  No fluxo do processo empresarial do Processo de Vendas, abra o estágio **Qualificar**. Insira *\$800.000* como o orçamento estimado.
5.  O Fluxo do Processo Empresarial terá quatro estágios: **Qualificar**, **Desenvolver**, **Propor** e **Fechar**. O estágio Confirmar Interesse não fará parte do processo se o Valor do Orçamento for inferior a \$1.000.000.
6.  Mude o **Valor do Orçamento** para *\$1.200.000.*
7.  O Fluxo do Processo de Empresarial agora terá cinco estágios: **Qualificar**, **Confirmar Interesse**, **Desenvolver**, **Propor** e **Fechar**. Passe do estágio Qualificar para o próximo estágio.
8.  **Salve** a oportunidade.
9.  Selecione o estágio **Qualificar** e clique no botão **Próximo Estágio** para ir para o estágio **Confirmar Interesse**.
10. Confirme o interesse clicando em **Não** e depois em **Sim**.
11. Clique no botão **Próximo Estágio** para passar para o estágio **Desenvolver**.
12. Confirme se o campo Pontos problemáticos do cliente aparece na parte inferior do estágio Desenvolver.
13. Insira *As máquinas atuais não conseguem processar o volume do cliente* no campo Pontos problemáticos do cliente.
14. Selecione **Próximo estágio**.
15. **Salve** o registro.

