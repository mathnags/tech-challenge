# Tech Challenge – Fase 1: apoio ao diagnóstico de câncer de mama com Machine Learning

Projeto de classificação que usa medidas de exames de imagem (punção aspirativa por agulha fina) para estimar se um tumor de mama é **maligno** ou **benigno**. O objetivo é **apoiar** a triagem médica. A decisão final é sempre do profissional de saúde.

## Sobre os dados

- **Dataset:** Breast Cancer Wisconsin (Diagnostic)
- **Origem:** UCI Machine Learning Repository, disponibilizado no Kaggle pelo usuário **uciml**
  - Kaggle: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
  - UCI: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
- **Tamanho:** 569 pacientes × 33 colunas
- **Alvo:** `diagnosis` — `M` (maligno, 212 pacientes, 37%) ou `B` (benigno, 357 pacientes, 63%)
- **Features:** 30 medidas numéricas dos núcleos celulares (raio, textura, perímetro, área, suavidade, compacidade, concavidade, pontos côncavos, simetria e dimensão fractal), cada uma em três versões: média (`_mean`), erro padrão (`_se`) e pior valor (`_worst`)
- **Colunas que não são features:**
  - `id`: identificador do paciente
  - `Unnamed: 32`: coluna vazia (100% nula), gerada pela formatação do arquivo

O arquivo original está em `data/raw/data.csv` e **é versionado neste repositório** (≈ 125 KB) para que o projeto rode — inclusive via Docker — sem nenhum passo manual de download. Ele nunca é editado à mão: toda limpeza é feita por código.

## Estrutura do projeto

```text
tech-challenge-fase1/
├── data/
│   ├── raw/              # dados originais, sem alteração
│   └── processed/        # dados tratados, gerados pelo código
├── notebooks/            # análise exploratória (EDA) e experimentos
├── src/                  # código reutilizável: preparação, treino e avaliação
├── models/               # modelo treinado salvo
├── reports/
│   └── figures/          # gráficos usados no relatório
├── requirements.txt      # dependências do projeto
├── Dockerfile            # ambiente reprodutível para executar o pipeline
└── README.md
```

## Como executar

_Em construção._

## Metodologia

_Em construção._

## Resultados

_Em construção._

## Limitações e uso responsável

_Em construção._ O modelo é uma ferramenta de **apoio**: não substitui o diagnóstico médico.

## Vídeo de apresentação

_Em construção._
