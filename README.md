# Projeto de Testes Automatizados com Cypress e Cucumber

Este projeto é uma automação de testes utilizando **Cypress** e **Cucumber** para validar funcionalidades do site [Advantage Online Shopping](https://advantageonlineshopping.com). A automação inclui testes tanto para a interface web quanto para as APIs fornecidas pelo site.

## 🎯 **Objetivo do Projeto**

O objetivo é validar diferentes cenários de busca de produtos e atualização de imagens de produtos usando os seguintes endpoints da API:

- **GET**: `/catalog/api/v1/products/search`
- **PUT**: `/catalog/api/v1/product/image/{userId}/{source}/{color}`

Os testes verificam a integridade dos dados retornados, o status code das respostas e o comportamento esperado do sistema.

---

## 🛠️ **Configuração do Ambiente**

### **Pré-requisitos**

- **Node.js** (v14 ou superior)
- **Git**
- Extensão **Cucumber** para Cypress

### **Instalação do Projeto**

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd nome-do-projeto
   ```

3. Instale as dependências:
   ```bash
   npm install
   ```

4. Execute o Cypress:
   ```bash
   npx cypress open
   ```

---

## 📁 **Estrutura do Projeto**

```
cypress
|-- e2e
|   |-- features
|   |   |-- busca-produto.feature
|   |   |-- api
|   |       |-- busca-produto.feature
|-- fixtures
|   |-- example.json
|-- support
|   |-- commands.js
|   |-- e2e.js
node_modules
cypress.config.js
package.json
README.md
```

## ⚙️ **Comandos Importantes**

| Comando                 | Descrição                              |
|-------------------------|----------------------------------------|
| `npm install`           | Instala as dependências do projeto     |
| `npx cypress open`      | Abre a interface gráfica do Cypress    |
| `npx cypress run`       | Executa os testes em modo headless     |

---

## 🚀 **Executando os Testes**

### **Via Interface Gráfica (Cypress GUI):**

1. Execute o comando:
   ```bash
   npx cypress open
   ```

## ✅ **Validações Realizadas nos Testes**

1. **Busca de Produto:**
   - Validação do status code da resposta.
   - Verificação se os produtos retornados correspondem ao termo de busca.

2. **Atualizar Imagem do Produto:**
   - Validação do status code da resposta.
   - Verificação se a imagem do produto foi atualizada corretamente.
   - Validação do ID da imagem retornado.

---

## 🧩 **Extensões Utilizadas**

- `cypress-cucumber-preprocessor`

Para instalar:
```bash
npm install --save-dev cypress-cucumber-preprocessor
```

---

## 📚 **Documentação Oficial**

- [Cypress Documentation](https://docs.cypress.io/)
- [Cucumber Documentation](https://cucumber.io/docs/)
- [Advantage Online Shopping API Docs](https://www.advantageonlineshopping.com/api/docs/)

