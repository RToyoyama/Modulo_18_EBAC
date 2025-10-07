# Projeto: Regressão Linear no Mercado Imobiliário

Este projeto é uma aplicação prática das técnicas de regressão linear simples e múltipla, com foco em prever o valor de aluguel de imóveis a partir de variáveis como metragem, número de quartos e demais características estruturais. O objetivo é analisar desempenho de modelos preditivos, tratar outliers de modo robusto e refletir sobre desafios de generalização no ciclo de Ciência de Dados[attached_file:1].

## Objetivo

- Construir e avaliar modelos de regressão linear (simples e múltipla) utilizando dados de imóveis.
- Explorar o impacto das variáveis independentes no valor de aluguel.
- Diagnosticar problemas como overfitting, multicolinearidade e propor soluções práticas[attached_file:1].

## Descrição dos Dados

O conjunto inclui variáveis como:
- ValorAluguel, ValorCondominio, Metragem, NQuartos, NVagas, NBanheiros, NSuites.
- Os dados possuem alguns outliers devido à presença de imóveis de luxo; são tratados via winsorização pelo IQR ou percentil, sem exclusão de amostras[attached_file:1].

## Fluxo Principal do Projeto

1. **Exploração e tratamento de dados**
   - Winsorização pelo IQR para outliers extremos (ex: aluguel, metragem), evitando distorção nas médias.
   - Estratégia por percentil para variáveis discretas (banheiros, suítes).
2. **Visualização e análise**
   - Estatísticas descritivas, boxplots e análise de correlação.
3. **Modelagem**
   - Separação em treino e teste.
   - Ajuste de regressão linear simples (apenas metragem) e múltipla (todas as variáveis).
   - Exposição dos coeficientes e formulação das equações dos modelos.
4. **Validação**
   - Métricas \( R^2 \) para treino e teste.
   - Discussão sobre generalização, multicolinearidade e overfitting[attached_file:1].

## Principais Resultados

- A métrica metragem foi um forte preditor (alto \( R^2 \) no treino de regressão simples, mas desempenho limitado em teste).
- Modelo múltiplo apresentou \( R^2 \) altíssimo no treino, mas não generalizou, indicando overfitting e multicolinearidade.
- Recomenda-se o uso de regularização (Ridge, Lasso) ou seleção de variáveis para cenários similares[attached_file:1].


