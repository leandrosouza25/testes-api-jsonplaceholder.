# 🧪 Automação de Testes de API - JSONPlaceholder

Projeto de automação de testes End-to-End (E2E) desenvolvido para validar os principais endpoints (GET, POST, PUT, DELETE) da API pública JSONPlaceholder.

## 🛠️ Tecnologias Utilizadas
* **Postman:** Criação e validação dos scripts de teste.
* **Newman:** Execução dos testes via linha de comando (CLI).
* **Newman Reporter HTML Extra:** Geração de relatórios visuais com gráficos.
* **GitHub Actions:** Automação e execução dos testes em uma esteira de CI/CD.

## 🚀 Como rodar o projeto localmente

1. Instale as dependências:
   ```bash
   npm install -g newman newman-reporter-htmlextra
   ```
2. Execute os testes:
   ```bash
   newman run collection.json --env-var "base_url=https://jsonplaceholder.typicode.com" -r htmlextra --reporter-htmlextra-export ./report.html
   ```
