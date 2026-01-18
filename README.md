# Pipeline ETL com Python - Desafio DIO Santander Bootcamp

## 📋 Descrição

Este projeto é um desafio prático do **Bootcamp de Data Science da DIO em parceria com o Santander**, focado na implementação de um **pipeline ETL (Extração, Transformação e Carregamento)** utilizando Python.

O objetivo principal é demonstrar o fluxo completo de dados através das três etapas fundamentais:
- **Extract (Extração)**: Leitura de dados de um arquivo CSV
- **Transform (Transformação)**: Manipulação e enriquecimento dos dados
- **Load (Carregamento)**: Persistência dos dados processados

## 🎯 Objetivos

- Compreender e aplicar os conceitos de **ETL**
- Manipular dados com **Pandas**
- Trabalhar com estruturas de dados JSON
- Demonstrar habilidades práticas em Ciência de Dados com Python

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **Pandas**: Manipulação e análise de dados
- **Requests**: Requisições HTTP (preparado para integração com APIs)
- **JSON**: Manipulação de dados estruturados
- **OpenAI API**: Integração preparada para geração de conteúdo com IA (opcional)

## 📂 Estrutura do Projeto

```
Desafio_ETL/
│
├── Desafio_Pipeline_ETL_Python.ipynb    # Notebook principal com o pipeline ETL
├── desafio_etl_dio_santander_sample.csv # Arquivo de dados de entrada
├── desafio_etl_dio_santander_atualizado.csv # Arquivo de saída com dados processados
└── README.md                             # Este arquivo
```

## 🔄 Fluxo do Pipeline ETL

### 1. **Extract (Extração)**
- Leitura do arquivo CSV com dados de usuários
- Carregamento dos dados em um DataFrame do Pandas

### 2. **Transform (Transformação)**
- Adição de novos usuários à base de dados existente
- Estruturação de dados bancários:
  - Informações de conta (número, agência, saldo, limite)
  - Informações de cartão (número, limite)
  - Notícias e features personalizadas
- Preparação de mensagens personalizadas (com suporte para integração com IA)

### 3. **Load (Carregamento)**
- Salvamento dos dados transformados em um novo arquivo CSV
- Validação e verificação dos dados processados

## 📊 Estrutura dos Dados

Os dados de usuários contêm os seguintes campos:

| Campo | Descrição |
|-------|-----------|
| `id` | Identificador único do usuário |
| `name` | Nome do usuário |
| `account_id` | ID da conta bancária |
| `account_number` | Número da conta |
| `account_agency` | Agência bancária |
| `account_balance` | Saldo da conta |
| `account_limit` | Limite da conta |
| `card_id` | ID do cartão |
| `card_number` | Número do cartão (mascarado) |
| `card_limit` | Limite do cartão |
| `features` | Funcionalidades disponíveis |
| `news` | Notícias e mensagens personalizadas |

## 🚀 Como Executar

### Pré-requisitos

```bash
# Instalar as dependências necessárias
pip install pandas requests
```

### Execução

1. Clone este repositório
2. Certifique-se de que o arquivo `desafio_etl_dio_santander_sample.csv` está no diretório correto
3. Abra o notebook `Desafio_Pipeline_ETL_Python.ipynb`
4. Execute as células sequencialmente

### Opcional: Integração com OpenAI

Para utilizar a geração de mensagens com IA:

```bash
pip install openai
```

Configure sua chave de API:
```python
openai.api_key = 'SUA_CHAVE_DE_API_AQUI'
```

> **Nota**: A integração com OpenAI está preparada no código, mas não foi utilizada neste projeto para evitar custos adicionais.

## 📈 Resultados

O pipeline processa com sucesso:
- ✅ Leitura de dados de usuários existentes
- ✅ Adição de novos usuários (Lia e Rafa)
- ✅ Estruturação completa de dados bancários
- ✅ Geração de arquivo CSV atualizado
- ✅ Validação dos dados processados

## 🔍 Principais Funcionalidades

1. **Carregamento de Dados**: Leitura eficiente de arquivos CSV
2. **Manipulação de DataFrames**: Uso de Pandas para operações de dados
3. **Concatenação de Dados**: Adição de novos registros mantendo a integridade
4. **Estruturação JSON**: Trabalho com dados estruturados em formato JSON
5. **Persistência de Dados**: Salvamento de dados processados

## 📚 Referências

- [Notebook Original do Desafio](https://github.com/falvojr/santander-dev-week-2023/blob/master/SantanderDevWeek2023.ipynb)
- [Documentação Pandas](https://pandas.pydata.org/)
- [OpenAI API Documentation](https://platform.openai.com/docs/api-reference/introduction)

## 👨‍💻 Autor

Desenvolvido como parte do **Bootcamp Santander 2026 - DIO**

## 📝 Licença

Este projeto é de código aberto e está disponível para fins educacionais.

---

⭐ Se este projeto foi útil para você, considere dar uma estrela!
