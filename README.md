
# Elasticsearch Autocomplete Hands-On

Este repositório contém um conjunto de notebooks para demonstrar como configurar e utilizar o Elasticsearch para tarefas práticas como instalação local, operações CRUD, e implementação de autocomplete com análise `edge_ngram`.

## :open_file_folder: Estrutura dos Notebooks

### `01-Install.ipynb`
Script de instalação rápida do Elasticsearch e Kibana via Docker, fornecido pela própria Elastic. Ao final do processo, você terá:

- Elasticsearch acessível em `http://localhost:9200`
- Kibana em `http://localhost:5601`
- Usuário padrão: `elastic`
- Senha e chave de API fornecidas automaticamente

[🔗 Documentação oficial da instalação local](https://github.com/elastic/start-local)

---

### `03-HandsOn.ipynb`
Demonstrações práticas utilizando a biblioteca Python `elasticsearch`. Inclui:

- Leitura e processamento de dados de cursos da Alura
- Criação de índices no Elasticsearch
- Operações básicas de CRUD
- Verificação de conexão com o cluster

---

### `04-Autocomplete.ipynb`
Implementação do recurso de **autocomplete** com `edge_ngram`, abordando:

- Conceito de `n-gram` e `edge_ngram`
- Imagens explicativas da tokenização
- Definição de `analyzer` personalizado
- Mapeamento de campo com `autocomplete` e `autocomplete_search`
- Inserção de dados no índice configurado

---

## :computer: Requisitos

- Docker (para rodar Elasticsearch e Kibana localmente)
- Python 3.8+
- Bibliotecas:
  - `elasticsearch`
  - `pandas`
  - Jupyter

Você pode instalar as dependências com:

```bash
pip install -r requirements.txt
```

---

## :rocket: Executando os Notebooks

1. Certifique-se de que Elasticsearch está rodando localmente (`http://localhost:9200`)
2. Abra o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Navegue pelos arquivos na ordem: `01-Install`, `03-HandsOn`, e `04-Autocomplete`

---

## :memo: Créditos

Este material foi desenvolvido para fins educacionais e demonstrações práticas sobre Elasticsearch.
