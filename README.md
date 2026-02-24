# 📱 Redes Sociais e Saúde Mental
### Uma Análise Estatística do Comportamento de Estudantes

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-lightblue?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-teal)
![SQLite](https://img.shields.io/badge/SQL-SQLite-orange?logo=sqlite)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

---

## 📌 Sobre o Projeto

Este projeto analisa o comportamento de **705 estudantes de 10 países** em relação ao uso de redes sociais e seus impactos na saúde mental, qualidade do sono e desempenho acadêmico.

A análise foi estruturada como um projeto de dados completo — da exploração dos dados até recomendações orientadas ao negócio — utilizando Python para análise estatística e SQL para consultas analíticas.

---

## 🎯 Perguntas de Negócio

1. Qual o perfil de uso — quantas horas por dia, quais plataformas, qual o nível de dependência?
2. Uso intensivo está associado a pior saúde mental e menos horas de sono?
3. Existe diferença de comportamento entre níveis acadêmicos e gêneros?
4. Uso excessivo impacta o desempenho acadêmico? Os estudantes percebem isso?
5. Qual plataforma está mais associada a altos níveis de dependência?

---

## 📊 Principais Resultados

| Insight | Resultado |
|---|---|
| Correlação uso × saúde mental | ρ = −0.80 (muito forte, p < 0.001) |
| Correlação uso × sono | ρ = −0.81 (muito forte, p < 0.001) |
| Estudantes com uso > 5h/dia | 47,4% (IC 95%: 43,7% – 51,1%) |
| Relatam impacto no desempenho | 64,3% dos estudantes |
| Estudantes em zona de risco | 9,6% (múltiplos critérios combinados) |

> **Conclusão principal:** Quanto maior o tempo de uso diário de redes sociais, pior a saúde mental, menos horas de sono e maior o score de dependência — todas as relações estatisticamente significativas.

---

## 📋 Conteúdo do Notebook

**1. Configuração e Carregamento**
Importações, configuração visual e carregamento do dataset.

**2. Análise Exploratória (EDA)**
Estatísticas descritivas, distribuições das variáveis quantitativas (histogramas + boxplots) e distribuição das variáveis qualitativas (gênero, nível acadêmico, plataformas).

**3. Análise Estatística**
- Correlação de Spearman entre uso, saúde mental, sono e dependência
- Teste de hipótese com t de Student
- Intervalo de confiança (95%) para proporção de uso intensivo
- Teste Qui-Quadrado: associação entre gênero e nível acadêmico
- Mapa de correlação geral (heatmap)

**4. Análise SQL com SQLite**
5 queries analíticas demonstrando uso real de SQL:
- Perfil médio por nível acadêmico
- Top 5 plataformas por dependência média
- Segmentação por nível de uso com CTE
- Estudantes em zona de risco com múltiplos critérios
- Ranking por plataforma e gênero com Window Function (`ROW_NUMBER OVER PARTITION BY`)

**5. Conclusões e Dashboard**
Painel visual com os principais insights e recomendações orientadas ao negócio.

---

## 🛠️ Ferramentas e Bibliotecas

| Ferramenta | Uso |
|---|---|
| `Pandas` | Manipulação e análise dos dados |
| `Seaborn` / `Matplotlib` | Visualizações |
| `SciPy` | Testes estatísticos (Spearman, Qui-Quadrado) |
| `NumPy` | Cálculos numéricos |
| `SQLite3` | Análise SQL integrada ao notebook |

---

## 📂 Dataset

**Students' Social Media Addiction**
- **Fonte:** [Kaggle](https://www.kaggle.com/datasets/adilshamim8/social-media-addiction-vs-relationships)
- **Registros:** 705 estudantes
- **Países:** 10 (Bangladesh, Brasil, Índia, EUA, UK, Alemanha, Austrália, Canadá, Coreia do Sul, Japão)
- **Período:** 1º trimestre de 2025
- **Variáveis utilizadas:** 9 de 13 disponíveis

---

## ⚠️ Limitações

- Dados autodeclarados — sujeitos a viés de resposta
- Amostra desbalanceada por nível acadêmico (apenas 27 estudantes do ensino médio)
- Correlação não implica causalidade — fatores externos não mensurados podem influenciar os resultados

---

## 👩‍💻 Autora

**Maria Gabriela Martins de Souza**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-blue?logo=linkedin)](https://linkedin.com/in/mgabrielamnts)
[![GitHub](https://img.shields.io/badge/GitHub-Perfil-black?logo=github)](https://github.com/mgabrielamnts)
