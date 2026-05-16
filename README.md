[README.md](https://github.com/user-attachments/files/27822834/README.md)
# Análise Estatística do Brilho Estelar — Simulação, Inferência e Outliers

**************************************************************************
Professores Orientadores: Sérgio Monteiro, D.Sc.; Manuel Martins, D.Sc.

Aluna: Marja Tanita de Oliveira Ramos gringel
**************************************************************************

Este projeto realiza uma análise estatística completa sobre dados simulados de brilho estelar. 
O objetivo é verificar se os dados seguem o modelo teórico assumido, aplicar métodos de inferência e avaliar o impacto de outliers.


## Objetivos do Projeto

- Simular 1000 observações de brilho estelar seguindo uma distribuição normal.
- Visualizar a distribuição dos dados por meio de histogramas, boxplots e QQ-plots.
- Calcular estatísticas descritivas básicas.
- Construir intervalos de confiança (IC) para a média.
- Realizar testes de hipótese (t e z) comparando a média amostral com a média teórica.
- Identificar outliers usando métodos estatísticos (IQR e Z-score).
- Avaliar o impacto dos outliers na média.
- Interpretar os resultados de forma pedagógica.

## Metodologia

1. **Simulação dos dados** 
 Os dados foram gerados usando `rnorm()`, assumindo:
 - média teórica: 15.5 
 - desvio padrão do telescópio: 0.8 
 - tamanho da amostra: 1000 

2. **Visualização** 
 Foram criados:
 - Histograma com densidade e curva normal teórica 
 - Boxplot 
 - QQ-plot 

3. **Inferência estatística** 
 - Estatísticas descritivas 
 - Intervalos de confiança (t e z) 
 - Teste t 
 - Teste z manual 

4. **Diagnóstico de outliers** 
 - Método do IQR (1.5 × IQR) 
 - Método do Z-score (|z| > 3) 
 - Comparação da média com e sem outliers


## Estrutura do Notebook

1. **Simulação dos Dados**  
   Geração da amostra e criação do data frame.

2. **Visualização da Distribuição**  
   Gráficos para avaliar normalidade e possíveis valores extremos.

3. **Inferência Estatística**  
   ICs, testes t e z, e estatísticas descritivas.

4. **Outliers**  
   Identificação, análise e impacto na média.

5. **Conclusão**  
   Síntese dos resultados e interpretação final.


## Resultados Resumidos

- A média amostral ficou muito próxima da média teórica (15.5).
- Os intervalos de confiança (t e z) incluíram o valor teórico.
- Os testes t e z apresentaram valores-p altos → **não rejeitamos H0**.
- Os dados simulados são compatíveis com a distribuição normal assumida.
- Outliers foram identificados pelos métodos IQR e Z-score.
- A média sem outliers ficou ainda mais próxima da média teórica.
- Outliers podem distorcer a média e aumentar a variabilidade.


## Como Executar

1. Abra o notebook no Google Colab.
2. Execute a célula de instalação de pacotes **apenas se necessário**.
3. Execute as células em ordem.
4. Observe os gráficos, tabelas e interpretações.


## Conclusão

A análise confirma que os dados simulados seguem adequadamente o modelo normal proposto.  
Os intervalos de confiança e testes de hipótese mostram que a média amostral é compatível com o valor teórico.  
A identificação de outliers evidencia que valores extremos podem influenciar a média e o desvio padrão, reforçando a importância de reportar resultados **com e sem outliers**.

O estudo demonstra como ferramentas estatísticas podem validar modelos teóricos e avaliar a qualidade dos dados.
