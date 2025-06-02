## 📄 Relatório Release I

### Atividades Realizadas

1. Organização e Estruturação Inicial
    - Atualização do `README.md`.
    - Adição do `CONTRIBUTING.md` com as diretrizes de contribuição.
    - Definição de licença (`LICENSE`) e código de conduta (`CODE_OF_CONDUCT.md`).
    - Padronização do repositório:
        - Implementação de templates de Pull Requests e Issues.
        - Aplicação de versionamento de software.

2. Implementação de Pipeline CI/CD
    - Build automatizado.
    - Execução de lint.
    - Execução de testes.

🔗 **Releases Publicadas:**

- [gov-hub v1.0.0](https://github.com/gces-govhub/gov-hub/releases/tag/v1.0.0)

- [app-lappis-ipea v1.0.0](https://github.com/gces-govhub/app-lappis-ipea/releases/tag/v1.0.0)

- [infra-lappis-ipea v1.0.0](https://github.com/gces-govhub/infra-lappis-ipea/releases/tag/v1.0.0)

---

### Análise da Arquitetura Existente

Realizamos uma análise da arquitetura de dados atual do projeto:

- **Camada Bronze:**
    - Dados brutos das tabelas.

- **Camada Silver:**
    - Dados integrados e estruturados.

Identificamos que:

- A coluna `observação` da Tabela B contém informações não estruturadas com identificadores relevantes (NF, contrato, processo).
- As Tabelas A e B são integradas utilizando essas informações para formação da Tabela Silver.
- O projeto utiliza **Apache Airflow** para orquestração do ETL e **DBT** para transformação dos dados.

---

### Definição da Estratégia de Implementação

Com base na análise realizada, definimos que:

- A **extração automática dos identificadores** será realizada durante o processo de transformação no DBT.
- Um **script Python** será invocado no momento da transformação via:
    - Macros DBT
    - Ou DBT Python Models (`dbt-python-model`)
- Utilizaremos um **modelo de NER** (Named Entity Recognition) baseado em **HuggingFace Transformers (BERTimbau)** para identificar e extrair os campos automaticamente.

---
