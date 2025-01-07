### **ReadMe para o Projeto**

# **Análise de Cotações de Ações e Índices Financeiros**

Este projeto utiliza **Python** para analisar cotações históricas de índices e ações de mercado financeiro. As informações são obtidas por meio da biblioteca **yfinance**, e os resultados são apresentados em tabelas e gráficos.

---

## **Funcionalidades**

1. **Obtenção de Cotações:**
   - Baixa dados históricos de cotações de índices e ações do Yahoo Finance.
   - Exibe os dados em tabelas para visualização.

2. **Visualização Gráfica:**
   - Gera gráficos da evolução do preço de fechamento dos ativos selecionados.

3. **Leitura de Empresas de um Arquivo Excel:**
   - Lê uma tabela com tickers de empresas e baixa automaticamente as cotações para cada uma.

---

## **Tecnologias Utilizadas**

- **Python 3.7+**
- **Bibliotecas:**
  - `pandas`: Manipulação de dados.
  - `matplotlib`: Geração de gráficos.
  - `yfinance`: Obtenção de dados financeiros do Yahoo Finance.
  - `openpyxl`: Leitura de arquivos Excel.

---

## **Pré-requisitos**

1. Instale o Python e as dependências do projeto:
   ```bash
   pip install pandas matplotlib yfinance openpyxl
   ```

2. Prepare o arquivo **Empresas.xlsx**:
   - Deve conter uma coluna chamada **'Empresas'** com os tickers das ações ou índices a serem analisados.
   - Exemplo de conteúdo do arquivo:

     | Empresas  |
     |-----------|
     | PETR4.SA  |
     | VALE3.SA  |
     | ITUB4.SA  |

---

## **Como Utilizar**

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu_usuario/nome_do_repositorio.git
   cd nome_do_repositorio
   ```

2. Certifique-se de que o arquivo **Empresas.xlsx** está no mesmo diretório do código.

3. Execute o script:
   ```bash
   python script.py
   ```

---

## **Explicação do Código**

1. **Cotações Específicas**:
   - Baixa e plota as cotações do índice **Bovespa** (`^BVSP`) e das ações da **Petrobras** (`PETR4.SA`) para o período de 01/01/2020 a 01/01/2021.

2. **Leitura do Arquivo Excel**:
   - Lê a tabela de tickers do arquivo **Empresas.xlsx**.

3. **Iteração sobre as Empresas**:
   - Para cada empresa listada no Excel:
     - Obtém as cotações históricas para o período de 01/01/2023 a 01/01/2024.
     - Exibe os dados na tela.
     - Gera um gráfico do preço de fechamento.

---

## **Exemplo de Saída**

1. **Tabela de Dados:**
   | Data       | Open   | High   | Low    | Close  | Volume   |
   |------------|--------|--------|--------|--------|----------|
   | 2020-01-02 | 118573 | 118736 | 117652 | 118854 | 10000000 |

2. **Gráfico:**
   - Um gráfico mostrando a evolução do preço de fechamento no período selecionado.

---

## **Licença**
Este projeto é de uso livre, sob a licença MIT. Sinta-se à vontade para utilizá-lo e adaptá-lo conforme necessário.

---
