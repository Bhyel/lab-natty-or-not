# 🚀 Startup Pitch Generator

## Do Brainstorm ao Conceito Visual em Minutos (Powered by AWS PartyRock)

---

## 🌟 Descrição do Projeto

O **Startup Pitch Generator** é uma aplicação *no-code* criada para acelerar a fase de validação inicial de ideias de negócio. 

Ao invés de gastar horas formatando um conceito, o usuário insere a ideia central e a aplicação gera instantaneamente os três elementos fundamentais para um *kick-off* de sucesso:

1.  **Análise SWOT** completa.
2.  **Elevator Pitch** persuasivo (30 segundos).
3.  **Conceito Visual de Logo** e Branding.

O objetivo é transformar uma simples inspiração em um conceito formal e apresentável, utilizando o poder da IA Generativa.

---

## 🛠️ Tecnologias e Ferramentas

| Categoria | Componente | Detalhes |
| :--- | :--- | :--- |
| **Plataforma Principal** | AWS PartyRock | Playground *no-code* para desenvolvimento de aplicações de IA. |
| **Modelos de Base (FMs)** | Amazon Bedrock | Utiliza modelos de ponta como **Anthropic Claude** (texto) e **Stability AI** (imagem). |
| **Widgets** | `Input de Texto`, `Generated Text`, `Generated Image` | Elementos de interface e geração de conteúdo. |

---

## ⚙️ Processo de Criação (Engenharia de Prompt Encadeada)

O diferencial deste projeto reside no **encadeamento lógico de prompts**, onde a saída de um widget alimenta o próximo, garantindo profundidade e consistência.

### 1. Definição da Entrada (Input Principal)

* **Widget:** `Input de Texto`
* **Título:** `Minha Ideia de Negócio`

### 2. Criação da Análise SWOT

* **Widget:** `Generated Text` (1)
* **Título:** `Análise SWOT Express`
* **Prompt Chave:**
  ```
  Gere uma Análise SWOT (Forças, Fraquezas, Oportunidades, Ameaças) completa para a ideia: @Minha Ideia de Negócio. Apresente em formato de lista simples e clara, sem rodeios.
  ```
    

### 3. Refinando o Elevator Pitch (Encadeamento de 2 Widgets)

* **Widget:** `Generated Text` (2)
* **Título:** `Elevator Pitch (30 Segundos)`
* **Prompt Chave (Avançado):**
    ```
    Com base na ideia: @Minha Ideia de Negócio, e usando os principais insights da análise: @Análise SWOT Express, crie um discurso de venda (pitch) de 30 segundos. Foco em quem você ajuda, qual problema resolve e o diferencial da solução.
    ```

### 4. Conceito Visual e Branding

* **Widget:** `Generated Image`
* **Título:** `Conceito de Logo/Branding`
* **Prompt Chave:**
    ```
    Crie um conceito de logo minimalista, moderno e digital para a ideia: @Minha Ideia de Negócio. Use uma paleta de cores vibrante.
    ```

---

## ✨ Resultados e Exemplos

| Entrada de Exemplo | Saída Resumida |
| :--- | :--- |
| **"Plataforma de aluguel de itens de festa de vizinhança."** | **SWOT:** Identificou **Força** (Comunidade Engajada) e **Fraqueza** (Logística). |
| | **Pitch:** Gerou um discurso envolvente, focado no aspecto de **uso único** dos itens. |
| | **Visual:** Entregou um ícone estilizado combinando uma casa e um balão de festa. |

Link Para utilização: https://partyrock.aws/u/Narcand/SQVieLMjl/new-app-SQVieLMjl

---

## 💭 Reflexão (O Desafio No-Code)

O sucesso deste projeto depende totalmente da **Engenharia de Prompt Encadeada** (como visto no item 3). Foi crucial instruir o modelo a **utilizar a saída do widget `@Análise SWOT Express`** para criar um pitch mais fundamentado, em vez de apenas repetir a ideia inicial.

Isso ensina que, mesmo em ambientes *no-code* como o PartyRock, a arquitetura lógica e a qualidade dos prompts são a nova "codificação".



## Links Interessantes

[Base10: If You’re Not First, You’re Last: How AI Becomes Mission Critical](https://base10.vc/post/generative-ai-mission-critical/)

![Base10's Trend Map Generative AI](https://github.com/digitalinnovationone/lab-natty-or-not/assets/730492/f4df26e8-f8f7-4419-8252-c69d73ea930c)
