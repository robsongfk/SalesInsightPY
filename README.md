# SalesInsight PY
Mini projeto SCTEC

## Sobre o projeto
Análise e visualização de dados de vendas desenvolvida em Python. O projeto carrega, limpa, transforma, agrega e visualiza um dataset de vendas, gerando métricas por período, produto, categoria e região, além de uma segmentação simples de clientes por faixa de gasto.

## O que o projeto analisa
- Receita total e volume de vendas por mês e por trimestre
- Top produtos e categorias por receita
- Desempenho por região
- Segmentação de clientes por nível de gasto (Bronze, Prata, Ouro)
- Relação entre quantidade vendida e receita por transação
- Exportação de relatórios em CSV e JSON e de gráficos em PNG

## Conceitos aplicados (Módulo 01 - Semanas 01 a 08)
- Lógica de programação: variáveis, tipos, operadores, condicionais
- Estruturas de dados: listas, tuplas, dicionários e compostas
- Funções: parâmetros, retorno, docstrings, lambda, ordem superior[cite: 1]
- Leitura e escrita de arquivos CSV e JSON[cite: 1]
- Módulo datetime e expressões regulares (re)[cite: 1]
- Pandas: Series, DataFrames, filtros, groupby, transformações[cite: 1]
- NumPy: arrays, operações vetorizadas e broadcasting[cite: 1]
- Matplotlib e Seaborn: linha, barra, dispersão, subplots, export[cite: 1]
- Introdução a classes: construtor, atributos e métodos[cite: 1]
- Git e GitHub: branches, commits e GitFlow simplificado[cite: 1]

## Como executar
**Google Colab (Recomendado)**
1. Abra o arquivo `salesinsight.ipynb` diretamente no Google Colab.
2. Vá em **Ambiente de execução** > **Executar tudo**.
3. O fluxo completo será executado automaticamente, desde a geração do arquivo sintético `vendas.csv` até a exportação dos relatórios e gráficos na pasta `outputs/`.

## Decisões técnicas
- **Uso do `np.select` e operações vetorizadas:** Optamos por utilizar o `np.select` do NumPy em vez de laços `for` tradicionais para criar a coluna de "Faixa de Receita". Isso garante melhor performance por conta da vetorização nativa em grandes volumes de dados.
- **Estruturação em Classe:** Todo o pipeline analítico foi encapsulado na classe `AnalisadorDeVendas` para facilitar a manutenção, o reaproveitamento do código e a orquestração via método `main()`.
- **Tratamento de Strings com Regex:** Utilizamos a biblioteca `re` para garantir a extração segura de caracteres alfanuméricos e formatar rigorosamente o padrão de clientes, evitando falhas silenciosas na agregação de dados.

## Ferramentas utilizadas
- Python 3.10+[cite: 1]
- Google Colab[cite: 1]
- Bibliotecas: pandas, numpy, matplotlib, seaborn, re, json, datetime, os, random[cite: 1]
- GitHub para versionamento[cite: 1]
- Kanban para gestão visual do projeto[cite: 1]

## Vídeo de demonstração
[COLE O LINK DO SEU VÍDEO AQUI]
