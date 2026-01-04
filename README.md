# 📊 Xbox Game Pass – Análise de Vendas

Este projeto realiza a análise das vendas de assinaturas do Xbox Game Pass, utilizando dados reais de assinantes, planos, valores e benefícios extras como EA Play e Minecraft Season Pass. O objetivo é gerar insights sobre o desempenho mensal das vendas, segmentar por tipo de plano e criar visualizações dinâmicas para facilitar a tomada de decisão.

## 📁 Dados Utilizados

O arquivo principal é o **dashboard_finalizado.xlsx**, que contém:

*   **Assinantes:** ID, nome, plano, data de início, mês/ano, renovação automática, valor da assinatura, tipo de assinatura.
*   **Benefícios Extras:** Indicação de aquisição do EA Play Season Pass e Minecraft Season Pass, com respectivos valores.
*   **Cálculos:** Tabelas dinâmicas com somatórios de vendas por tipo de plano, auto renovação e mês.
*   **Dashboard:** Painel visual com gráficos e segmentações para análise rápida.

## 🛠️ Como Reproduzir

1.  **Clone este repositório:**
    ```bash
    git https://github.com/MaximillerGuedes/Desafio-Dashboard-de-Vendas.git
    cd xbox-gamepass-analise
    ```

2.  **Abra o arquivo `dashboard_finalizado.xlsx` no Excel (versão 2010 ou superior):**
    *   Navegue até a aba de dados de assinaturas.
    *   Caso queira criar uma coluna auxiliar "Mês/Ano", insira uma nova coluna e utilize a fórmula:
        ```excel
        =TEXTO([@Start Date];"mm/aaaa")
        ```
    *   Arraste a fórmula para todas as linhas.

3.  **Crie uma Tabela Dinâmica:**
    *   Selecione toda a base de dados.
    *   Vá em **Inserir > Tabela Dinâmica**.
    *   Use a coluna "Mês/Ano" como rótulo de linha e "Total Value" como valor (soma).

4.  **Adicione Segmentação de Dados:**
    *   Com a tabela dinâmica selecionada, clique em **Analisar > Inserir Segmentação de Dados**.
    *   Escolha "Mês/Ano" para filtrar facilmente os resultados.

5.  **Crie um Gráfico Dinâmico:**
    *   Selecione a tabela dinâmica e insira um gráfico de colunas ou barras.
    *   Copie o gráfico para a aba **Dashboard** para visualização centralizada.

## 📈 Resultados Esperados

*   Visualização clara das vendas mensais.
*   Filtros dinâmicos para análise por período.
*   Gráficos intuitivos para apresentação em reuniões ou relatórios.

## 🤝 Contribuição

Sinta-se à vontade para abrir issues, sugerir melhorias ou enviar pull requests!
