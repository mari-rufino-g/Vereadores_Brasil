
 # Vereadoras - Por candidaturas competitivas

Este repositório contém um simples projeto de Data Science desenvolvido para embasar um trabalho para a disciplina Sistemas políticos, partidários e eleitorais do curso Mídia, Política e Sociedade que realizo na FESPSP. O projeto foi realizado utilizando a linguagem python e diversas bibliotecas específicas da área de Data Science sendo as principais:

* 	Pandas: - Para importação e exploração dos dados;
* 	Seaborn:  - Para visualização dos dados;
* 	Matplotilib: – Para produção de gráficos
* 	Geopandas: - Para visualização de dados espaciais e georreferenciados
Estudei sobre as cotas eleitorais para mulheres e seus impactos nas eleições para o cargo de vereador. 


## 🚀 Objetivo

Em 2018, o TSE determinou que os partidos deveriam destinar ao menos 30% do fundo eleitoral para candidaturas de mulheres com a intenção de tornar essas candidaturas mais competitivas. Para verificar o impacto desta resolução analisei e comparei os dados dos resultados das eleições municipais em todo o território nacional em 2016 (antes da lei) e em 2020 (após a lei).

### 📋 Perguntas a serem respondidas?

De que coisas você precisa para instalar o software e como instalá-lo?

```
1.	A lei mencionada provocou aumento do número de vereadoras eleitas em 2020 se comparado a 2016?
```
```
2.	Em que medida a sub-representação das mulheres pode ser atribuída à baixa oferta de candidatas?
```
```
3.	Em 2016 e 2020, o investimento na candidatura de vereadores foi maior do que para mulheres?
```
```
4.	Existe alguma relação entre região brasileira e proporção de mulheres nas câmaras municipais? 
```

### 🔧 Estrutura dos dados

O TSE disponibiliza em seu site dois arquivos sobre os resultados das eleições: um sobre o resultado em si e outro sobre os dados dos candidatos. 

* **•	Consulta de candidatos por zona eleitoral:**  63 colunas em que há dados como estado civil, gênero, bens declarados, número do partido, idade, ocupação, cor/raça, grau de instrução, email, cpf, cidade, valor gasto para campanha, etc.
* **•	Resultados da votação por zona eleitoral por candidato:**  38 colunas com dados sobre a candidatura tais como numero do partido, quantidade de votos obtidos,  município, estado, cargo (prefeito ou vereador), código de município, partido político, coligação, etc. 
* **•	Shapefile do Brasil** - Para produção do mapa

Foi preciso mesclar os dois dataframes (candidatos e resultado das eleições) já que queria verificar os resultados das urnas levando em consideração o gênero dos candidatos. Selecionei as seguintes colunas: 

```
'SG_UF', 'NM_MUNICIPIO', 'NM_CANDIDATO','NR_CPF_CANDIDATO','DS_CARGO', 'NM_URNA_CANDIDATO', 'SG_PARTIDO', 'DS_GENERO', 'QT_VOTOS_NOMINAIS','VR_DESPESA_MAX_CAMPANHA', 'DS_SIT_TOT_TURNO','CD_MUNICIPIO'
```

Realizei este processo para os anos de 2016 e 2020 e filtrei somente os dados referente a candidaturas de vereadores já que a decisão do TSE não incide sobre cargos do executivo. Por fim, utilizei o shapefile do Brasil para produção do mapa.

## ⚙️ Metodologia

Foi realizada uma análise inicial dos dados (AED) com o objetivo de obter insights dos dados e respostas para as perguntas norteadoras do trabalho. 

## 🖇️ Resultados

![Lkd2](https://user-images.githubusercontent.com/80469682/124503200-6c34c880-dd9b-11eb-864f-a24cfed83ef9.png)


## 📌 Conclusão

Não se pode afirmar que as mudanças foram provocadas pela decisão do TSE sobre a distribuição partidária, mas ao comparar todos os dados obtidos a partir dos resultados das eleições de 2020 em relação a 2016 é possível afirmar que houve uma melhora no que diz respeito às candidaturas de mulheres conforme dados compilados acima. Se "não há no mundo nenhum motivo para negar à mulher o exercício do direito de votar ou a participação na criação e na administração da lei do país" é preciso garantir às mulheres candidaturas competitivas para que possam participar de fato sobre a incidência política, sobre a seleção de candidaturas, decisões partidárias, distribuição de recursos. Elas precisam poder escolher pela participação dos processos de tomada de decisão e isso não se faz com apenas 30% de recursos do fundo partidário.

## 🛠️ Referências

* [Dados eleitorais](https://www.tse.jus.br/eleicoes/estatisticas/repositorio-de-dados-eleitorais-1/repositorio-de-dados-eleitorais) - Base de dados para análise
* [Fundo Partidário - 30% para mulheres](https://www.tse.jus.br/imprensa/noticias-tse/2020/Agosto/acoes-do-tse-valorizam-participacao-da-mulher-na-politica-e-incentivam-candidaturas-femininas) - TSE aprova exigência de 30% do fundo partidário para candidaturas femininas

## ✒️ Autoria

Mariana Rufino

---



