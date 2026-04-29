# Análise Exploratória de Dados — Fatores que Impactam o NPS em um E-commerce

Este projeto realiza uma **Análise Exploratória de Dados (EDA)** completa com o objetivo de entender **quais fatores operacionais realmente impactam a satisfação do cliente**, medida pelo NPS (Net Promoter Score).

Mais do que visualizar dados, este trabalho busca **investigar causas reais da insatisfação**, utilizando abordagem analítica, validação de hipóteses e pensamento crítico.

O foco da análise não está no desenvolvimento do código, mas sim em investigação e entendimento do que está sendo apresentado.

Durante a análise também foram levantados pontos sobre a qualidade e confiabilidade dos dados.

---

## Objetivo do Projeto

O objetivo principal do projeto era responder a pergunta:

> **Quais fatores operacionais do e-commerce mais influenciam o NPS?**

Esse objetivo foi alcançado durante a análise. Além disso dados foram revelando informações onde pudemos obter ainda mais insights.

---

## Abordagem Analítica

A análise não segue um fluxo descritivo comum. O notebook foi estruturado como uma **investigação analítica**, passando por:

1. Entendimento da distribuição do NPS
2. Classificação de clientes por perfil (Detratores, Neutros, Promotores)
3. Teste de hipóteses clássicas
4. Criação de um método objetivo para identificar variáveis mais relevantes
5. Comparação entre dois perfis de detratores (nota 0 vs 3–6)
6. Investigação regional
7. Tentativa de correlação entre NPS e recompra
8. Identificação de inconsistências nos dados de recompra

---

## Principais Descobertas

### Atraso na entrega é o principal fator associado ao NPS

Clientes detratores apresentam, em média, **3,3x mais atraso** que promotores.

Mais do que isso:

- Clientes nota **0** tiveram ~4 dias de atraso
- Clientes nota **3–6** tiveram ~2 dias de atraso

Isso revela um **limite de tolerância do cliente**. A partir de certo ponto, a frustração vira insatisfação extrema.

---

### Atendimento ao cliente atua como “amortecedor” da experiência negativa

Mesmo com problemas logísticos, um bom atendimento reduz a chance do cliente se tornar nota 0.

---

### O tempo total de entrega importa menos que o atraso

O prazo final é quase igual entre clientes 0 e 3–6.  
O que realmente pesa é o **descumprimento da promessa**.

---

### O problema não está no perfil do cliente

Idade, região e tempo de relacionamento têm impacto mínimo.  
O problema é **operacional**, não demográfico.

---

### A análise de recompra revelou inconsistência nos dados

Ao tentar correlacionar NPS com recompra em 30 dias, foi identificado um padrão estatisticamente impossível.

Essa etapa demonstra maturidade analítica ao reconhecer que **os dados não permitem essa conclusão**.

---

## Insights Extras

Durante a EDA, os dados foram revelando mais informações que ao investigar conseguimos informações valiosas como:

> **O que faz um cliente se tornar um detrator extremo (nota 0) em vez de apenas um cliente frustrado (nota 3–6)?**

> **É possível saber o NPS necessário para manter o cliente comprando?**

--

## Estrutura do Projeto

O projeto possui dois arquivos principais:
- Um notebook onde é mostrado passo a passo a análise, explicando insights que conseguimos e decisões tomadas em cada etapa
- Uma apresentação de slides menos técnica com o objetivo de mostrar as informações de forma clara e direta a uma audiência não-tecnica.

### Estrutura de Pastas:

.<br>
├── data/<br>
│ └── desafio_nps_fase_1.csv<br>
├── notebooks/<br>
│ └── eda.ipynb<br>
├── reports/<br>
│ └── slide/<br>
│   └── apresentacao_slides.pptx<br>
├── src/<br>
├── README.md<br>
├── .gitignore<br>
└── requirements.txt<br>
