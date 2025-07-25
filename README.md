# Guardião das Tartaruguinhas 🐢
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Licença](https://img.shields.io/badge/Licença-MIT-green)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

Um sistema em Python puro para fortalecer a conservação comunitária de quelônios na Amazônia, através do monitoramento de ninhos.

---

## 📖 Tabela de Conteúdos
1. [Sobre o Projeto](#-sobre-o-projeto)
2. [Funcionalidades](#-funcionalidades)
3. [Como Executar](#-como-executar)
4. [Fluxograma da Aplicação](#-fluxograma-da-aplicação)
5. [Estrutura dos Dados](#-estrutura-dos-dados)
6. [Motivação e Contexto](#-motivação-e-contexto)
7. [Autor](#-autor)


---

### 📍 Sobre o Projeto

O **Guardião das Tartaruguinhas** é uma ferramenta de linha de comando que permite a voluntários de projetos de conservação registrar, consultar, editar e analisar dados sobre ninhos de quelônios. Ele transforma anotações de campo em uma base de dados estruturada e persistente (`dados_ninhos.csv`), sendo projetado para ser robusto, acessível e funcionar sem bibliotecas externas complexas.

**Interface do Programa:**

### ✨ Funcionalidades

-   **Menu Interativo:** Navegação guiada por um menu numérico simples, utilizando a estrutura `match...case`.
-   **Persistência de Dados:** Todos os registros são salvos em um arquivo `.csv`, garantindo que os dados não sejam perdidos.
-   **Inicialização Inteligente:** Se nenhum arquivo de dados for encontrado, o sistema cria um com 10 registros de exemplo.
-   **Operações CRUD Completas:**
    -   **Criar:** Inserir registros de novos ninhos.
    -   **Ler:** Visualizar relatórios e estatísticas detalhadas.
    -   **Atualizar:** Editar informações de um ninho existente.
    -   **Deletar:** Excluir um registro, com passo de confirmação para segurança.
-   **Validação de Dados:** Previne a entrada de dados inválidos (ex: ovos negativos, status incorreto).
-   **Análise e Relatórios:** Gera estatísticas e um gráfico de distribuição em modo texto para fácil visualização.

### ▶️ Como Executar

#### **Pré-requisitos**
* Python 3.10 ou superior.

#### **Método 1: Localmente**
1. Baixe o arquivo `guardiao.py` (ou o nome que você deu ao script).
2. No seu terminal, navegue até a pasta do arquivo.
3. Execute o comando:
   ```sh
   python guardiao.py
