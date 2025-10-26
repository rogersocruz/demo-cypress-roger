# Projeto de Testes End-to-End com Cypress (Micro-Livraria)

Este repositório é um fork do projeto [aserg-ufmg/demo-cypress](https://github.com/aserg-ufmg/demo-cypress), desenvolvido como parte da atividade prática sobre testes end-to-end (E2E) da disciplina de Engenharia de Software.

O objetivo foi implementar um conjunto de testes E2E usando Cypress para simular a interação de um usuário com uma aplicação de "micro-livraria", validando o fluxo completo de compra de um livro.

Este `README.md` serve como a documentação principal do projeto, detalhando como configurar o ambiente e executar os testes.

---

## 🚀 Configuração e Execução (Passo a Passo Detalhado)

Para executar o projeto, utilizamos o Docker para "containerizar" tanto a aplicação (front-end e back-end) quanto o executor de testes (Cypress). Isso garante um ambiente consistente e isolado.

### Passo 1: Construir a Imagem da Aplicação

Primeiro, precisamos construir a imagem Docker que contém o back-end (Node.js) e o front-end (Web) da micro-livraria.

**Comando:**
(Execute na raiz do projeto, onde está o `README.md`)
```bash
docker build -t micro-livraria -f cypress/Dockerfile .
