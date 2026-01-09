# Projeto Pós 1

## 📋 Sobre o Projeto

Sistema de processamento de dados implementando a arquitetura Medallion (Bronze-Silver-Gold), desenvolvido como projeto inicial para exploração e validação de pipelines de transformação de dados utilizando DuckDB.

## 🚀 Tecnologias

- **Python** - Linguagem principal
- **DuckDB** - Banco de dados analítico
- **Pandas** - Manipulação e análise de dados
- **Jupyter Notebook** - Desenvolvimento interativo
- **Poetry** - Gerenciamento de dependências
- **VS Code** - Ambiente de desenvolvimento

## 📦 Instalação

### Pré-requisitos

- Python 3.8+
- Poetry

### Passos

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/Projeto_pos_1.git

# Acesse o diretório
cd Projeto_pos_1

# Instale as dependências com Poetry
poetry install

# Ative o ambiente virtual
poetry shell
```

## 💻 Uso

O projeto utiliza notebooks Jupyter para processamento de dados em etapas:

```bash
# Execute os notebooks na seguinte ordem:
# 1. Ingestão de dados (Bronze)
jupyter notebook scripts/ingestao.ipynb

# 2. Refinamento de dados (Silver)
jupyter notebook scripts/refinamento.ipynb

# 3. Enriquecimento de dados (Gold)
jupyter notebook scripts/enriquecimento.ipynb

# Ou execute o pipeline completo
jupyter notebook notebook/pipeline.ipynb
```

## 📁 Estrutura

```
Projeto_pos_1/
├── .venv/              # Ambiente virtual
├── data/               # Camadas de dados (Medallion Architecture)
│   ├── bronze/         # Dados brutos
│   ├── silver/         # Dados limpos e transformados
│   └── gold/           # Dados agregados e enriquecidos
├── landing/            # Arquivos CSV de origem
│   ├── z0019_1.csv
│   └── z0019_2.csv
├── notebook/           # Pipeline completo
│   └── pipeline.ipynb
├── scripts/            # Notebooks de processamento
│   ├── ingestao.ipynb        # Camada Bronze
│   ├── refinamento.ipynb     # Camada Silver
│   ├── enriquecimento.ipynb  # Camada Gold
│   └── dados_duckdb.db.wal   # DuckDB Write-Ahead Log
├── pyproject.toml      # Configuração Poetry
└── README.md
```

## 🏗️ Arquitetura Medallion

O projeto segue a arquitetura de três camadas:

- **Bronze (Landing → Bronze)**: Ingestão de dados brutos dos arquivos CSV
- **Silver (Bronze → Silver)**: Limpeza, validação e transformação dos dados
- **Gold (Silver → Gold)**: Agregações e enriquecimento para análise de negócio

## 🤝 Contribuições

Contribuições são bem-vindas! Por favor:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

## ✒️ Autor

**Daniel** 

[text](https://www.linkedin.com/in/daniel-mec/)

---

Desenvolvido com 💙 para fins educacionais