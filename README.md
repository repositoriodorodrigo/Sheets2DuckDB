# Sheets2DuckDB

# Pipeline de Processamento de Dados Google Sheets para DuckDB com Google Colab e Visualizações no Google Data Studio

Este projeto demonstra um pipeline de processamento de dados que extrai informações de uma planilha do Google Sheets, utiliza o Google Colab para ingerir e transformar os dados com as bibliotecas gspread, pandas e pyduckdb, disponibiliza os dados transformados no DuckDB e cria visualizações interativas no Google Data Studio. Além disso, automatiza o processamento diário usando o Google Apps Script para acionar o pipeline.

## Objetivo

O objetivo deste projeto é criar um fluxo automatizado para processar, transformar e visualizar dados de uma planilha do Google Sheets, utilizando ferramentas do ecossistema Google e compartilhando os resultados por meio de visualizações interativas.

## Fluxo do Pipeline

1. **Extração de Dados do Google Sheets:**
   - Utiliza a biblioteca gspread para extrair os dados da planilha do Google Sheets.

2. **Transformação com o Google Colab:**
   - Um notebook do Google Colab é usado para realizar transformações nos dados extraídos.
   - A biblioteca pandas é utilizada para a manipulação e limpeza dos dados.
   - A biblioteca pyduckdb é utilizada para interagir com o DuckDB e executar transformações SQL.

3. **Armazenamento no DuckDB:**
   - Os dados transformados são armazenados no DuckDB, um banco de dados otimizado para análises interativas.

4. **Criação de Visualizações com o Google Data Studio:**
   - O DuckDB é conectado ao Google Data Studio para criar visualizações interativas e painéis de análise.

5. **Automação com Google Apps Script:**
   - O Google Apps Script é usado para agendar e acionar o pipeline de processamento diariamente, processando os dados de D-1.

## Configuração e Uso

1. Instale as dependências necessárias no ambiente do Google Colab:
   ```bash
   # Instale a biblioteca gspread
   !pip install gspread
   
   # Instale a biblioteca pandas
   !pip install pandas
   
   # Instale a biblioteca pyduckdb
   !pip install pyduckdb

## Configuração e Uso

1. **Execução do Notebook do Google Colab (`data_processing_pipeline.ipynb`):**
   - Siga as instruções no notebook para autenticar-se com a API do Google Sheets e implementar as etapas de extração, transformação e armazenamento no DuckDB.

2. **Configuração do Google Data Studio:**
   - Acesse o Google Data Studio e crie um novo relatório.
   - Conecte-se ao DuckDB como fonte de dados.
   - Crie visualizações interativas utilizando os dados armazenados.

3. **Configuração do Google Apps Script:**
   - Crie um projeto no Google Apps Script.
   - Implemente um script para acionar o pipeline diariamente, utilizando um gatilho de tempo.

## Estrutura do Projeto

- `notebooks/`: Contém o notebook do Google Colab (`data_processing_pipeline.ipynb`) com o código de extração, transformação e armazenamento.
- `data/`: Armazena arquivos CSV de exemplo ou intermediários (se necessário).
- `docs/`: Documentação do projeto, capturas de tela e outros recursos.

## Resultados

- Dados transformados armazenados no DuckDB.
- Visualizações interativas criadas no Google Data Studio.

## Recursos Adicionais

- [Documentação do Google Sheets API](https://developers.google.com/sheets/api)
- [Documentação do gspread](https://gspread.readthedocs.io/en/latest/)
- [Documentação do pandas](https://pandas.pydata.org/docs/)
- [Documentação do DuckDB](https://duckdb.org/docs)
- [Google Data Studio](https://datastudio.google.com/)
- [Google Apps Script](https://developers.google.com/apps-script)

## Contribuição

Contribuições são bem-vindas! Se você encontrar problemas ou quiser melhorar este pipeline, sinta-se à vontade para enviar um pull request.
