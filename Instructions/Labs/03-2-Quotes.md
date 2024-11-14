---
lab:
  title: 'Laboratório 3.2: Criar cotações'
---

# Módulo 3: Gerenciar pedidos e o catálogo de produtos com o Dynamics 365

## Laboratório Prático 3.2 – Criar cotações

### Cenário
Como analista de vendas da implementação do Dynamics 365 Sales na Contoso Coffee, você deseja garantir que os vendedores possam aproveitar os aprimoramentos do catálogo de produtos durante todo o ciclo de vida de vendas. Para garantir que a funcionalidade esteja funcionando corretamente, você testará o processo de criação de uma cotação de uma nova oportunidade.

Após a conclusão bem-sucedida deste laboratório, você poderá:
- Criar oportunidades e adicionar itens de linha de oportunidade
- Criar uma cotação de uma oportunidade

### Exercício 1 – Criar uma cotação

#### Tarefa 1 – Adicionar itens de linha de produtos
Nesta tarefa, você criará uma Oportunidade e adicionará Itens de linha de produtos.
1. Vá para o aplicativo Hub de Vendas do Dynamics 365.
2. No menu à esquerda, no grupo Vendas, selecione **Oportunidades.**
3. Clique em **+ Novo**.
4. Insira *Interessado em acessórios do Airpot XL* para Tópico e selecione **Jon Doe** para Contato.
5. No cabeçalho do registro na parte superior, selecione a **seta para baixo** ao lado do campo Proprietário e escolha **Test Coffee Shop, Inc.** para Conta. Selecione **Salvar**.
6. Selecione a guia **Produtos**.
7. Você deve selecionar uma Lista de preços antes de adicionar Produtos de oportunidade. Selecione **Filtrar direto** para Lista de preços.
8. Selecione **Calculado pelo sistema** para receita.
9. Acima da subgrade, clique em **+ Adicionar produtos.**
10. Na lista Todos os produtos, encontre **Filtro de 6 meses do Airpot XL**, digite *6* para Quantidade, selecione **Adicionar.**
11. Encontre **extensor de pote AirpotXL** na lista de produtos, digite *1* para Quantidade e selecione **Adicionar.**
12. Encontre **Extensão do reservatório do Airpot XL** na lista de produtos, digite *1* para Quantidade e selecione **Adicionar.**
13. Você verá que três produtos foram adicionados. Selecione **Salvar**.
14. Clique duas vezes no produto **Filtro de 6 meses do Airpot XL**.
15. Localize o campo Desconto por volume. Você verã que não há desconto.
16. Altere a Quantidade para *15* e clique fora do campo. O desconto agora entrará em vigor e o campo Desconto por volume mostrará o valor com desconto.
17. Selecione **Salvar e Fechar**.

#### Tarefa 2 – Criar cotação
Nesta tarefa, você criará uma Cotação da oportunidade criada na Tarefa 1.
1. Se ainda não estiver aberto, abra o aplicativo Hub de Vendas do Dynamics 365.
2. Se necessário, abra a oportunidade que você criou na tarefa anterior. Será chamado **Interessado em acessórios Airpot XL.**
3. Selecione a guia **Cotações**.
4. Acima da subgrade, clique em **+ Nova cotação.**
5. O formulário de cotação será aberto e as informações relevantes serão copiadas da oportunidade.
6. Na página Cotação de Interessado em acessórios do Airpot XL, examine a subgrade Produtos e certifique-se de que os produtos e suas quantidades estão conforme o esperado. Você pode alterar as quantidades e o desconto do preço de cada item de linha.
7. Na barra de comandos, selecione **Ativar cotação**. (Dependendo do tamanho do seu navegador, pode ser necessário selecionar as reticências para ver essa opção.)
8. Clique em **Exportar para PDF** localizado na barra de comandos e selecione **Imprimir cotação para o cliente.** Clique em **Download**.
9. Abra o documento gerado e veja como é a Cotação.
10. Feche o PDF.
11. Feche a janela Exportar para PDF.

