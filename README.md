
# 🔍 Projeto de Análise e Avaliação Automatizada de Repositórios com Google Gemini e GitHub

Este notebook permite realizar a **análise automática de repositórios GitHub**, utilizando agentes inteligentes baseados na API Google Gemini. Ele realiza:

- Análise de arquivos de código individualmente.
- Avaliação geral da estrutura do projeto.
- Sugestões de melhoria de código com boas práticas.
- Geração de Pull Requests com base nas análises.

---

## ⚙️ Pré-requisitos e Configuração

### 1. Clone ou abra este notebook no Google Colab

Clique em "Open in Colab" no topo do notebook ou suba o arquivo `.ipynb` diretamente.

---


### 2. Obtenha e configure suas chaves de API

#### 🔑 Google API Key (Gemini)

1. Acesse: [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
2. Copie sua chave de API.

#### 🔑 GitHub API Token

1. Vá até [GitHub Settings → Developer Settings → Personal Access Tokens](https://github.com/settings/tokens)
2. Gere um token com escopos: pull_requests:read/write, contents:read/write
3. 3. Copie a chave gerada.

#### 🔐 Definindo no ambiente Colab

Adiocione as Keys ao Colab

'GOOGLE_API_KEY' e 'GITHUB_API_KEY'
---

## ▶️ Instruções de uso

### Seleção de Repositório

1. O notebook listará seus repositórios públicos/privados disponíveis via GitHub API.
2. Selecione um deles usando o dropdown interativo.

### Etapas executadas:

- ✅ Leitura e exibição do `README.md` (se disponível)
- ✅ Análise recursiva de todos os arquivos de código
- ✅ Geração de relatório de avaliação técnica
- ✅ Criação da branch `evaluation` e envio de `evaluation.md`
- ✅ Geração de Pull Request automático

---

### Agente de Melhoria de Código

- Permite selecionar um arquivo específico do repositório
- O agente reescreve o conteúdo com boas práticas e docstrings
- Você pode criar um Pull Request com a versão sugerida pelo agente

---

## 🧠 Agentes disponíveis

- `analista_codigo`: Interpreta e explica arquivos de código.
- `avaliador_projeto`: Gera uma avaliação geral do projeto.
- `assistente_codigo`: Reescreve e melhora um arquivo específico.

---

## ✅ Funcionalidades automáticas

- Análise de estrutura e qualidade do projeto.
- Sugestões automatizadas e documentação.
- Criação de branches e Pull Requests via API do GitHub.
- Visualização interativa com IPython e Markdown.

---

## 📝 Observações

- O uso da API Gemini pode ter limites de cota gratuitos.
- Tokens do GitHub devem ser armazenados com segurança.
- Funciona melhor com repositórios bem estruturados e arquivos de código legíveis.

---

## 📄 Licença

Este notebook é distribuído sob licença MIT. Sinta-se à vontade para adaptá-lo conforme necessário.
