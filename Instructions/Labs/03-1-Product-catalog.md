---
lab:
  title: 'Laboratório 3.1: Configurar o catálogo de produtos'
---

# Módulo 3: Gerenciar pedidos e o catálogo de produtos com o Dynamics 365

## Laboratório prático 3.1: Gerenciar catálogo de produtos

### Cenário
À medida que a Contoso Coffee cresce, eles procuram padronizar sua estrutura de preços e permitir a criação mais fácil de cotações, pedidos e faturas com preços e detalhes de produtos mais precisos. Recentemente, a Contoso Coffee lançou sua máquina de café inteligente. Como consultor funcional na implementação do Dynamics 365 Sales, você foi solicitado a configurar o catálogo de produtos.

Após a conclusão bem-sucedida deste laboratório, você poderá:
- Criar grupos de unidades
- Definir listas de preços
- Criar listas de descontos
- Definir produtos e famílias de produtos

### Exercício 1 – Catálogo de produtos

#### Tarefa 1 – Criar grupo de unidades
Nesta tarefa, você criará grupos de unidades para uma linha de filtros de máquina de café.
1. Vá para o aplicativo Hub de Vendas do Dynamics 365.
2. Clique no menu Alterar área (localizado no canto inferior esquerdo da tela). Por padrão, Vendas será exibido na parte inferior do menu à esquerda.
3. No menu exibido, selecione **Configurações do Aplicativo**.
4. Selecione **Grupos de unidades** na seção Catálogo de produtos do menu à esquerda.
5. Clique em **+ Novo**.
6. Insira **Filtros** para Nome, insira **Cada um** para Unidade principal e clique em **OK.**
7. Quando o Grupo de unidades for aberto, selecione a guia Relacionado e escolha **Unidades.**
8. Você verá que só tem a unidade padrão Cada agora; você adicionará mais três unidades. Clique em **+ Nova unidade.**
9. Insira <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</bpt></bpt>Filtro<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</ept></ept> para Nome, <bpt ctype="x-unknown" id="3" rid="2"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</bpt></bpt>1<ept id="4" rid="2"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</ept></ept> para Quantidade, selecione <bpt ctype="x-unknown" id="5" rid="3"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</bpt></bpt>Cada<ept id="6" rid="3"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</ept></ept> para Unidade base e clique em <bpt ctype="x-unknown" id="7" rid="4"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</bpt></bpt>Salvar e criar novo<ept id="8" rid="4"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</ept></ept> ao selecionar o ícone de menu suspenso <bpt ctype="x-unknown" id="9" rid="5"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</bpt></bpt>˅<ept id="10" rid="5"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</ept></ept> à direita do botão Salvar e fechar.
10. Insira *Pacote* para Nome, *2* para Quantidade, selecione **Filtro** para Unidade base e clique em **Salvar e Criar Novo.**
11. Insira *Valor do pacote* para Nome, *2* para Quantidade, selecione **Pacote** para Unidade base e clique em **Salvar e fechar.**
12. Agora você deve ter quatro grupos de unidades na lista.

#### Tarefa 2 – Criar lista de descontos
Nesta tarefa, você criará uma Lista de descontos para pessoas que comprarem 15, 20 ou mais filtros. 15 filtros terão um desconto de 15% e 20 a 50 filtros terão um desconto de 25%.
1. Selecione **Listas de descontos** na seção Catálogo de produtos do menu à esquerda.
2. Clique em **+ Novo**.
3. Insira *Desconto de quantidade* para Nome, selecione **Porcentagem** para Tipo e clique em **Salvar.**
4. Clique em **Relacionado** e escolha **Descontos.**
5. Clique em **+ Novo desconto.**
6. Certifique-se de que Desconto por quantidade esteja selecionado para Tipo de desconto, insira *15* para Quantidade inicial, *19* para Quantidade final, *15* para Porcentagem e clique em **Salvar.**
7. Clique novamente em **+ Novo**.
8. Selecione **Desconto por quantidade** para Tipo de desconto. Em seguida, insira *20* para Quantidade inicial, *50* para Quantidade final, insira *25* para Porcentagem e clique em **Salvar.**

#### Tarefa 3 – Criar lista de preços
Nesta tarefa, você criará uma lista de preços para os filtros.
1. Selecione **Listas de preços** na seção Catálogo de produtos do menu à esquerda.
2. Clique em **+ Novo**.
3. Insira *Filtrar direto* para Nome, selecione **Dólar Americano** para Moeda e clique em **Salvar e fechar.**

#### Tarefa 4 – Criar produtos
Nesta tarefa, você criará os produtos.
1. Clique na área de alteração **Configurações do aplicativo**.
2. Selecione **Vendas.**
3. Selecione **Produtos** na seção Garantia do menu à esquerda.
4. Clique em **Adicionar produtos.**
5. Insira o *filtro de 6 meses do Airpot XL* para Nome, digite *AXL6MF-1234* para ID do produto (product ID), selecione **Filtros** para Grupo de unidades, selecione **Filtro** para Unidade padrão, digite *2* para Decimais suportados e clique em **Salvar.** (Talvez seja necessário selecionar a marca de seleção azul ao lado dos decimais suportados para aceitar a sugestão).
6. Selecione a guia **Detalhes adicionais**.
7. Clique nas **reticências verticais** no canto superior direito da seção Itens da lista de preços. Clique em **+ Novo item da lista de preços**.
8. Selecione **Filtrar direto** para Lista de preços, selecione **Desconto por quantidade** para Lista de descontos e selecione **Todo** para Opção de venda parcial.
9. Selecione a guia **Informações de preços**, insira *25* para Valor e selecione **Salvar e fechar.**
10. Se a publicação automática estiver ativada, ignore esta etapa. (Publicar não aparecerá na barra de comandos.) Caso contrário, selecione **Publicar** e **Confirmar** para publicar o produto.
11. No menu à esquerda, selecione **Produtos** no grupo Garantia.
12. Clique em **Adicionar produtos.**
13. Insira *Extensão de Reservatório Airpot XL* para Nome, digite *AXLRE-4321* para ID do produto (Product ID), selecione **Unidade Padrão** para Grupo de Unidades, selecione **Unidade Principal** para Unidade Padrão, selecione a marca de seleção azul ao lado de 2 para Decimais Suportados e clique em **Salvar.**
14. Selecione a guia **Detalhes adicionais**.
15. Clique nas **reticências verticais** no canto superior direito da seção Itens da lista de preços. Clique em **+ Novo item da lista de preços.**
16. Selecione **Filtrar direto** para Lista de preços. Selecione **Todo** para a opção de venda parcial.
17. Selecione a guia **Informações de preços**, insira *US$ 299* para Valor e selecione **Salvar e fechar.**
18. Se a publicação automática estiver ativada, ignore esta etapa. Caso contrário, selecione **Publicar** e **Confirmar** para publicar o produto.
19. Selecione **Produtos** no menu à esquerda.
20. Clique em **Adicionar produtos.**
21. Digite *Extensor Por Airpot XL* para Nome, digite *AXPLE-7894* para ID do produto (Product ID), selecione **Unidade Padrão** para Grupo de Unidades, selecione **Unidade Principal** para Unidade Padrão, selecione a marca de seleção azul ao lado de 2 para Decimais Suportados e clique em **Salvar.**
22. Selecione a guia **Detalhes adicionais**.
23. Clique nas **reticências verticais** no canto superior direito da seção Itens da lista de preços. Clique em **+ Novo item da lista de preços.**
24. Selecione **Filtrar direto** para Lista de preços. Selecione **Todo** para a opção de venda parcial.
25. Selecione a guia **Informações de preços**, insira *199* para Valor e selecione **Salvar e fechar.**
26. Se a publicação automática estiver ativada, ignore esta etapa. Caso contrário, selecione **Publicar** e **Confirmar** para publicar o produto.
27. Selecione **Produtos** no menu à esquerda.
28. Os produtos que você criou devem aparecer na visualização Todos os produtos, famílias e pacotes. Você pode alternar para essa exibição selecionando o ícone de menu suspenso <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> ao lado do título da exibição padrão. 
