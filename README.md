# ClearBank: Desafio final de Análise Financeira com Python

Desafio final do módulo **Análise de Dados e Inteligência de Negócios com IA da Faculdade Rocketseat - FTR**.

O projeto é um notebook Python que lê e valida um arquivo CSV de transações bancárias de uma fintech fictícia chamada ClearBank, agrupa os dados por mês, calcula métricas financeiras, sinaliza
movimentações suspeitas, exibe um relatório formatado no terminal e exporta o resultado em JSON.

A solução principal usa apenas a **biblioteca padrão do Python** (`csv`, `json`, `datetime`),
sem pandas. As versões com `pandas` e `matplotlib` entram como requisitos opcionais.

---

## Como executar

### Google Colab

1. Abra o `desafio-final.ipynb` no Colab.
2. Menu `Ambiente de execução` → `Executar tudo`.

A primeira célula recria o `transacoes.csv` automaticamente caso ele não esteja presente,
então o notebook roda de ponta a ponta sem upload manual.

### Jupyter local

```bash
git clone https://github.com/<seu-usuario>/clearbank-analise.git
cd clearbank-analise

pip install pandas matplotlib   # apenas para os requisitos opcionais

jupyter notebook desafio-final.ipynb
```

Execute as células **na ordem**, de cima para baixo.

Requer **Python 3.10 ou superior**.

### Versão com pandas (opcional)

```bash
python analise_pandas.py
```

---

## O que o notebook gera

| Arquivo | Conteúdo |
|---|---|
| `relatorio.json` | Relatório completo da análise (métricas mensais, período e transações suspeitas) |
| `grafico.png` | Crédito, débito e saldo por mês |

Além dos arquivos, o notebook imprime no terminal o resumo da limpeza dos dados, o relatório
mensal formatado em Real e a lista de transações suspeitas.

---
