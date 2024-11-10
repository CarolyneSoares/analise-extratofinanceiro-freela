# Análise de Extratos Financeiros com Python e Power BI




https://github.com/user-attachments/assets/ca106ea8-06eb-4100-b246-492dfa5c52ae


Este projeto foi desenvolvido como parte de um trabalho freelancer. A cliente solicitou a extração de informações financeiras de um PDF e a criação de um dashboard interativo para visualização dos dados. Para atender a essa demanda, utilizei **Python** para processar os dados e **Power BI** para criar o dashboard, permitindo uma análise detalhada e intuitiva.

## 1. Processamento de Dados com Python

**Ferramentas e Bibliotecas Utilizadas**: 
- **PyPDF2**: para leitura e extração de texto do PDF.
- **pandas**: para manipulação e organização dos dados em DataFrames.
- **regex** (expressões regulares): para identificar padrões no texto e extrair informações como datas e valores.

1. **Extração de Dados do PDF**
   - Utilizei a biblioteca **PyPDF2** para ler o PDF dos extratos financeiros.
   - Extraí informações como **datas**, **descrições**, **valores**, e **tipos de transação** (entrada/saída) usando expressões regulares para identificar e estruturar os dados.

2. **Organização dos Dados em DataFrame**
   - Criei um **DataFrame** com a biblioteca pandas para organizar as transações de forma estruturada.
   - Esse DataFrame permite análises mais detalhadas e a manipulação dos dados.

3. **Categorização de Receitas e Despesas**
   - Desenvolvi funções personalizadas para categorizar transações, distinguindo tipos específicos de receitas e despesas, como Pix, Boleto, Transferência, etc.
   - Gerei tabelas separadas para **receitas** e **despesas**, exportando cada uma para arquivos CSV, o que facilitou a análise posterior no Power BI.

4. **Cálculos Financeiros**
   - Calculei o **faturamento total**, **total de despesas** e o **lucro**, proporcionando uma visão geral das finanças.

## 2. Análise e Visualização no Power BI

Com os dados processados em Python, importei os arquivos CSV para o Power BI e realizei as seguintes configurações e transformações para criar um dashboard interativo.

**Ferramentas e Funcionalidades Utilizadas**:
- **Power BI Desktop**: para criação do dashboard e visualizações.
- **Medidas DAX**: para cálculos personalizados, como lucro, prejuízo e formatação condicional.

### Medidas Criadas

1. **Cor_Lucratividade**: Aplica uma formatação condicional para destacar a lucratividade com cores, facilitando a identificação visual do lucro.
2. **Cor_Lucro**: Define uma cor específica para valores de lucro, ajudando na diferenciação visual entre lucro e prejuízo.
3. **Lucro**: Calcula o lucro total como a diferença entre receitas e despesas.
4. **Lucro_Positivo**: Indica se houve lucro, permitindo análises de períodos lucrativos.
5. **Porcentagem_Lucratividade**: Calcula a porcentagem de lucratividade, mostrando o percentual de lucro em relação ao faturamento total.
6. **Prejuízo**: Quantifica o prejuízo nos períodos em que as despesas superaram as receitas.

### Tabelas de Dados

1. **Datas_Unificadas**: Criei uma tabela de datas unificadas para relacionar as datas de todas as transações, permitindo uma análise temporal eficiente no dashboard.
2. **total_despesas**: Tabela filtrada com todas as transações de saída (despesas), contendo informações como Data, Fornecedor/Destino, Tipo de Despesa e Valor_despesas.
3. **total_receitas**: Tabela filtrada com todas as transações de entrada (receitas), com informações sobre Cliente/Origem, Data, Tipo de Receita e valor_receita.

### Visualização Interativa

- Com essas medidas e tabelas, criei um dashboard interativo no Power BI que permite explorar os dados financeiros de forma dinâmica.
- A visualização apresenta gráficos, filtros e métricas que tornam a análise financeira intuitiva e detalhada, permitindo identificar tendências e padrões importantes no fluxo de caixa.

---

Este projeto demonstra habilidades em **extração de dados de PDF**, **manipulação de dados com pandas**, e **visualização de dados financeiros** no Power BI. Foi desenvolvido para atender uma demanda específica de uma cliente em um trabalho freelancer.

> **Nota:** Devido à presença de informações pessoais, o link do dashboard não está disponível publicamente. Em vez disso, incluí um vídeo demonstrativo que apresenta as funcionalidades e visualizações principais do dashboard, respeitando a privacidade dos dados da cliente.
