# Guardião das Tartaruguinhas 🐢
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Licença](https://img.shields.io/badge/Licença-MIT-green)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

Um sistema em Python puro para fortalecer a conservação comunitária de quelônios na Amazônia, através do monitoramento de ninhos.

---

## 📖 Tabela de Conteúdos
1. [Sobre o Projeto](#1-sobre-o-projeto)
2. [Funcionalidades](#2-funcionalidades)
3. [Estrutura dos Dados](#3-estrutura-dos-dados)
4. [Motivação e Contexto](#4-motivação-e-contexto)
5. [Autor](#5-autor)


---

### **1. Sobre o Projeto**

O **Guardião das Tartaruguinhas** é uma ferramenta de linha de comando que permite a voluntários de projetos de conservação registrar, consultar, editar e analisar dados sobre ninhos de quelônios. Ele transforma anotações de campo em uma base de dados estruturada e persistente (`dados_ninhos.csv`), sendo projetado para ser robusto, acessível e funcionar sem bibliotecas externas complexas.

**Interface do Programa:**

### **2. Funcionalidades**

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

### **3. Estrutura dos Dados (`dados_ninhos.csv`)**

| Coluna              | Tipo de Dado | Descrição                                                       |
| ------------------- | ------------ | --------------------------------------------------------------- |
| `id`                | `int`        | Identificador numérico único para o ninho.                      |
| `regiao`            | `string`     | Nome da praia ou área de monitoramento.                         |
| `quantidade_ovos`   | `int`        | Número de ovos contados no ninho.                               |
| `status`            | `string`     | Condição do ninho: "intacto", "ameaçado", ou "danificado".      |
| `risco`             | `string`     | Nível de risco visual: "🟢" (estável), "🟡" (observação), "🔴" (crítico). |
| `dias_para_eclosao` | `int`        | Estimativa de dias restantes para a eclosão dos ovos.           |
| `predadores`        | `boolean`    | Presença de predadores registrada (`True` ou `False`).          |


### **4. Motivação e Contexto**
Este projeto foi inspirado em iniciativas de conservação reais, como o **Projeto Pé-de-Pincha**, e no contexto da **COP30 em Belém**. A meta é criar uma ponte entre o conhecimento tradicional e a tecnologia acessível, empoderando comunidades locais com ferramentas que elas possam usar de forma autônoma.

### **5. Autor**
* **João Paulo da Silva Cardoso**

---
Distribuído sob a Licença MIT.
