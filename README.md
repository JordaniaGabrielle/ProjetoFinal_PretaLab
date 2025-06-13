# 🧪 Análise do Sistema Nacional de Informações sobre Saneamento (SNIS)

Este repositório contém o projeto final do ciclo formativo de IA do PretaLab e tem como objetivo analisar a situação do saneamento básico nos estados brasileiros e sua relação com indicadores de saúde pública. 

Através da integração dos dados do SNIS com as bases do DataSUS via BigQuery, investigamos se há correlação entre investimentos em saneamento e a taxa de mortalidade por doenças relacionadas à ausência de infraestrutura adequada.

---

## 👥 Integrantes do Grupo

Projeto desenvolvido no curso de Inteligência Artificial da Pretalab por:

| Nome               | GitHub                                                                 |
|--------------------|------------------------------------------------------------------------|
| Aliana Simões      | [alia](https://github.com/alia)                                        |
| Fernanda Brito     | [pherys](https://github.com/pherys)                                    |
| Izaura Souza       | [izaurahae](https://github.com/izaurahae)                              |
| Jordânia Gabrielle | [JordaniaGabrielle](https://github.com/JordaniaGabrielle)              |
| Karla Oliveira     | [kabianca](https://github.com/kabianca)                                |
| Mariana Freitas    | [marianafreitas13](https://github.com/marianafreitas13)                |
| Taís Guimarães     | [taisgb](https://github.com/taisgb)                                    |

---

## 🎯 Objetivo do Projeto

Avaliar a cobertura de saneamento básico no Brasil nos últimos 5 anos, identificar padrões regionais, analisar a evolução dos investimentos públicos e verificar a correlação entre os dados de saneamento e os índices de mortalidade por doenças evitáveis.

---

## ❓ Perguntas Norteadoras

- Qual é a cobertura de acesso à água potável e esgotamento sanitário nos estados brasileiros nos últimos 5 anos?
- Quais os 5 estados com maior cobertura de água e de esgoto?
- Como variou o investimento público ao longo dos anos por estado?
- Qual a natureza jurídica mais recorrente na prestação desses serviços?
- Qual a tendência da natureza jurídica das instituições gestoras nos últimos 5 anos?
- Como os indicadores de saneamento se correlacionam com índices de saúde?

---

## ⚙️ Metodologia

### 1. Coleta e Pré-processamento

- Utilização da biblioteca `basedosdados` para acessar dados via Google BigQuery.
- Dados do SNIS (1995 a 2021); o ano de 2022 foi excluído por inconsistência.
- Complementação com dados do DataSUS via BigQuery.

### 2. Tratamento dos Dados

- Normalização com `pandas`.
- Conversão de tipos e remoção de registros ausentes/inconsistentes.
- Agrupamento por estado e ano.

### 3. Análises Realizadas

- Cobertura de água e esgoto por estado.
- Frequência da natureza jurídica das prestadoras.
- Evolução de investimento público por estado.
- Top 5 estados com maior cobertura.
- Análise das regiões com maior déficit.
- Correlação com mortalidade por doenças de veiculação hídrica.

---

## 🛠️ Tecnologias Utilizadas

- **Python**
- **Google Colab**
- **Google BigQuery**
- `pandas`, `numpy` – manipulação de dados
- `matplotlib`, `seaborn`, `plotly` – visualização de dados
- `google.cloud.bigquery` – integração com BigQuery

---

## 📊 Resultados Destacados

- A cobertura de água potável é mais ampla que a de esgoto, principalmente nas regiões Norte e Nordeste.
- Rankings elaborados com foco na população urbana:

**Top 5 Cobertura de Água Potável**  
**Top 5 Cobertura de Esgotamento Sanitário**

- **Investimento público nos últimos anos:**
  - **Estável:** Distrito Federal
  - **Queda:** Acre, Alagoas, Espírito Santo, Goiás, Pernambuco, Rondônia, Roraima, São Paulo, Tocantins
  - **Crescimento:** Amazonas, Bahia, Ceará, Maranhão, Mato Grosso, Pará, Piauí, Rio Grande do Sul
  - **Oscilação:** Amapá, Minas Gerais, Mato Grosso do Sul, Paraíba, Paraná, Rio de Janeiro, Rio Grande do Norte, Santa Catarina, Sergipe

- **Natureza jurídica predominante:**  
  - Sociedade de Economia Mista com Administração Pública
  - Em seguida: Administração Pública Direta, Autarquias e Empresas Públicas

---

## 📚 Fontes de Dados

- **SNIS – Sistema Nacional de Informações sobre Saneamento**
- **SIH/SUS – Sistema de Informações Hospitalares**
- [Base dos Dados - BigQuery](https://basedosdados.org/)
- [Habitat Brasil – Doenças relacionadas ao saneamento](https://www.habitatbrasil.org.br/blog/saneamento-basico-e-saude.html)

---

## 📌 Conclusão

O estudo demonstrou uma correlação significativa entre a precariedade no saneamento e o aumento das taxas de mortalidade por doenças evitáveis, com destaque para as regiões Norte e Nordeste. A predominância de sociedades de economia mista na gestão dos serviços se manteve ao longo do tempo. 

A análise evidencia a necessidade de políticas públicas mais eficazes e investimentos contínuos em saneamento, reforçando sua importância como determinante social da saúde.

