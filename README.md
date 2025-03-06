# The Economic Impacts of Minimum Wage Increases in Europe

## Project Overview
The relationship between minimum wage increases and economic indicators like inflation, unemployment, and purchasing power parity (PPP) has been a long-standing debate among policymakers, economists, and labor advocates. In recent years, several European countries have implemented significant changes to their minimum wage policies, making it a timely issue to explore.

This project examines how changes in minimum wage levels impact three critical aspects of the economy. Specifically, the analysis focuses on answering the following research question: How do changes in minimum wage affect inflation, unemployment, and purchasing power parity across Europe?

This project combines time series analysis with visualizations in Tableau to examine data from various European countries. Some of the key questions this project addresses include:

- What trends have minimum wages followed in Europe over the past 14 years, and how have they varied across countries?
- How does the minimum wage relate to the PPP index in different countries, and how does this affect workers' real purchasing power?
- How does the relationship between minimum wage increases and inflation impact purchasing power   in different countries?
- Does an increase in minimum wage lead to higher unemployment rates due to the increased cost of hiring for businesses?


The findings presented in this analysis are especially relevant for governments and organizations considering the introduction or increase of minimum wage laws, providing data-driven insights into the broader economic implications.

## Data Sources

The data for this analysis was collected from Eurostat, the official statistical office of the European Union. The dataset includes multiple economic indicators:

- [Minimum Wage Levels (nominal and adjusted for PPP)](https://ec.europa.eu/eurostat/databrowser/view/earn_mw_cur/default/table?lang=en)
- [Harmonized Index of Consumer Prices (HICP)](https://ec.europa.eu/eurostat/databrowser/view/prc_hicp_manr__custom_15661910/default/table?lang=en)
- Inflation of Essential Goods (HICP link filtered by good)
- [PPP Index](https://ec.europa.eu/eurostat/databrowser/view/prc_ppp_ind/default/table?lang=en)
- [Total Population Unemployed (ages 20-64)](https://ec.europa.eu/eurostat/databrowser/view/une_rt_a__custom_15661932/default/table?lang=en)
- [Expenditure of GDP on Unemployment](https://ec.europa.eu/eurostat/databrowser/view/spr_exp_func__custom_15662006/default/table?lang=en&page=time:2023)

Data was cleaned, formatted, and structured to ensure compatibility with Tableau for visualization. 

## Key Findings

## Minimum Wage and Purchasing Power Parity (PPP)

One of the key questions in this analysis is whether or not an increase in the minimum wage translates into a higher real purchasing power for workers. To evaluate this, we compare:

- **Nominal minimum wage:** the official minimum wage set by each country in euros, standardized for consistency.
- **PPP-Adjusted Minimum Wage:** measure that adjusts the minimum wage based on purchasing power parity (PPP), allowing for fair comparisons between countries by considering differences in the cost of living. 
- **PPP Index:** a measure of how expensive a country is relative to others. A higher PPP Index means a higher cost of living, reducing the real value of wages. A lower PPP Index means the cost of living is lower, allowing wages to stretch further.

Minimum wages have experienced significant increases throughout the European countries on this dataset between 2010-2024. While some countries have had 
![min_wage_trend](https://github.com/juliamartin0/minimum-wage-impact/blob/main/min_wage_trends.png)

Between 2012 and 2023, wages increased across Europe. However, the real impact on purchasing power varies. The graph below highlights that a high nominal wage doesn’t always equal high purchasing power. For example, Ireland has a high nominal wage but also a high PPP index, making its workers' PPP-adjusted wages lower than countries like Belgium or the Netherlands.

![ppp_index](https://github.com/juliamartin0/minimum-wage-impact/blob/main/ppp%20index.png)

This creates a gap between minimum wage and the cost of living, leaving Irish workers with less real purchasing power compared to workers in countries like Spain or Poland. Despite these countries having much lower nominal wages, their minimum wage increases have outpaced the growth of their PPP index, giving their workers a stronger minimum wage relative to other countries.

In other words:

- A **higher PPP Index** than adjusted wages means workers' aren't keeping up with inflation or the rising costs, reducing purchasing power. As a result, workers may struggle to afford basic necessities, even if their nominal wages seem high. This scenario shows a disconnection between wage increases and the actual cost of living, causing workers' real purchasing power to be weaker than expected. In our graph, this situation applies to countries like Ireland, Lithuania, or Portugal among others.
- A **lower PPP Index** than adjusted wages, means that the cost of living in that country is relatively low compared to the increase in nominal minimum wages. This results in workers having greater purchasing power because their wages go further in terms of buying goods and services. In countries with lower living costs, workers may enjoy a higher standard of living even if their nominal wages are not as high as in other countries with higher living costs. This is the case for countries like Germany, the Netherlands, and Spain, among others.
- When the  **PPP Index closely aligns with adjusted wages**, wage increases match living costs, keeping purchasing power stable and allowing workers to afford a similar amount of goods and services over time. This is the case for countries like Luxembourg and France. 

After analyzing this graph, we can conclude that **an increase in the nominal minimum wage does not always lead to an improvement in workers' purchasing power**. If inflation and cost-of-living rises faster than the wage increase, purchasing power may decline, even though nominal wages are higher. Therefore, inflation plays a significant role in determining whether wage increases actually improve workers' purchasing power. 

## Minimum Wage and Inflation

In analyzing the relationship between minimum wage increases and inflation across various European countries, we can gain valuable insights into how changes in wages impact workers' real purchasing power. While nominal wage increases are important, the real effect on workers' living standards largely depends on how those wage changes compare to inflation. More specifically, inflation can be broken down into harmonized inflation (HICP), which reflects the overall price changes in a country, and inflation in essential goods (such as food, energy, and housing), which directly affects workers' daily living costs.

The graphs below compare the percentage changes in minimum wage and inflation across different countries. By analyzing this relationship, we can see whether wage increases are keeping up with or outpacing inflation and how that affects workers’ real purchasing power. 

From our analysis, we can conclude that the relationship between minimum wage increases and inflation plays a crucial role in shaping workers’ real purchasing power. While increasing nominal wages is a key mechanism to support workers' income, its real impact depends on how those increases compare to inflation—both overall inflation (Harmonized Index of Consumer Prices, HICP) and the inflation of essential goods (such as food, energy, and rent).

In general:

- If **wages increase at a higher rate than HICP**, workers are more likely to maintain or improve their purchasing power. This can happen in two ways:

    i. Wage growth is significantly higher than inflation → This directly increases purchasing power. This is the case of Germany. As we can see in the graphs, the wage increase in 2023 was 18%, while the increase in HICP was 6%. Even though the inflation of essential goods was overall really high, the fact that wages increased so much in 2023 allowed German workers to keep a good purchasing power that year.
  
  ![germany](https://github.com/juliamartin0/minimum-wage-impact/blob/main/min%20wage%20-%20hicp%20germany.png)

    ii. Even if HICP is high, essential goods inflation remains low → Since basic necessities take up a large portion of workers' expenses, keeping their essential goods inflation lower prevents a major loss in purchasing power. This is the case for countries like Spain or the Netherlands. If wage increases do not sufficiently outpace inflation, or if inflation in essential goods is high, workers are more likely to lose purchasing power.

![spain](https://github.com/juliamartin0/minimum-wage-impact/blob/main/min%20wage%20-%20hicp%20spain.png)

- If **wage increases do not sufficiently outpace HICP**, and at the same time, **essential goods inflation (food, rent, energy) rises even higher than HICP**, workers' real incomes shrink, reducing their ability to afford goods and services. Even with nominal wage increases, the rising cost of essentials forces workers to spend a larger share of their income on necessities, effectively weakening their purchasing power. Countries like Ireland experienced this scenario. While wages did increase (7,6%), they were not enough to fully offset rising essential goods costs, leading to a decline in real purchasing power for workers.

![ireland](https://github.com/juliamartin0/minimum-wage-impact/blob/main/min%20wage%20-%20hicp%20ireland.png)

Ultimately, while increasing wages can be a tool to protect or enhance purchasing power, it is not a guarantee; it must be balanced with inflation levels, particularly in essential goods, to ensure that workers truly benefit from higher wages.

While these general patterns hold true in most cases, it is important to acknowledge that other economic factors can influence the relationship between minimum wage increases and purchasing power:

- Tax policies, social security contributions, or debt levels can affect disposable income.
- Regional disparities mean that national averages don’t always reflect local realities.
- Inflation expectations and economic uncertainty can influence consumer behavior and purchasing power perceptions.
  
Belgium is one of these exceptions. In 2023 it presented 2,3% of HICP while wages only increased by 0,11% and still managed to maintain a good purchasing power. The reason Belgium did not lose purchasing power is mainly due to automatic wage indexation and the sharp decline in energy prices (electricity = -27,2 %, gas = -53,8%), which offset the effects of food (14,3%) and rent (5,9%) inflation. This case highlights that while the relationship between wage increases and inflation is generally strong, exceptions exist when additional economic policies and structural factors come into play.

![belgium](https://github.com/juliamartin0/minimum-wage-impact/blob/main/min%20wage%20-%20hicp%20belgium.png)

## Minimum Wage Increases and Unemployment Rates

One of the most debated topics in labor economics is whether increasing the minimum wage negatively affects employment levels. Traditional economic theory suggests that raising wages could lead to job losses, as higher labor costs might force businesses to cut jobs. However, when analyzing the data from multiple European countries as shown in the graph below, between 2010 and 2023, we observe a different trend:

- Over the last 14 years, **minimum wages have generally increased across all countries in the dataset**, following a steady upward trajectory.
- At the same time, unemployment rates have tended to decline, meaning that despite higher wages, labor markets have remained stable or even improved. While unemployment rates have followed a downward trend, some exceptions exist. For example, Greece experienced a rise in unemployment around 2013 due to its financial crisis, and many countries saw temporary spikes in unemployment in 2020-2021 due to the COVID-19 pandemic.
- While some countries experienced temporary declines or stagnation in minimum wages, the overall pattern remains a steady wage increase alongside falling unemployment.
- Countries with substantial minimum wage growth, such as Lithuania and Spain, have not seen sustained increases in unemployment.

| ![unemp_spain](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_spain.png) | ![unemp_lithuania](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_lithuania.png) |
|----------------------------|----------------------------|
| ![unemp_netherlands](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_netherlands.png) | ![unemp_greece](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_greece.png) |


Despite this general trend, unemployment levels still differ significantly across countries due to structural and economic factors beyond just wage policies. Here are some key insights:

- Spain and Greece have higher unemployment rates despite moderate minimum wages. This is influenced by structural issues such as past economic crises, rigid labor regulations, and labor market composition.
- Eastern European countries have low minimum wages but varied unemployment rates, partly due to worker migration to higher-paying Western European countries.
- Luxembourg is an exception, with very high wages and a low unemployment rate (3.6%). Its small size, strong economy, and high-skilled immigrant workforce explain this anomaly.

While inflation plays a role in shaping labor markets, broader economic conditions have a greater impact on how wages affect employment:

**1. Labor Market Flexibility**

- Countries like Germany and Poland have more flexible hiring and firing policies, which help maintain lower unemployment rates.
- In contrast, Spain faces structurally high unemployment due to temporary contracts and rigid labor laws that make it costly to hire and fire workers.

**2. Productivity and Labor Costs**

- Countries with high productivity, such as Belgium and the Netherlands, can sustain higher wages without negatively impacting employment.
- If the total labor cost (minimum wage + taxes + social security contributions) is too high, it can discourage hiring, particularly in lower productivity economies.

**3. Unemployment Benefits and Social Protections** (*see scatter plot below*)

- Countries that offer higher unemployment benefits tend to experience higher unemployment rates in the short term. This is because workers may feel comfortable waiting for a better job opportunity or a more lucrative position, knowing they can rely on financial support for a longer period. As a result, there is less urgency to secure employment quickly, leading to a phenomenon known as "unemployment search disincentive". This situation can contribute to a temporary increase in the unemployment rate but can also offer greater economic stability for unemployed individuals. They have the financial security to take their time finding a job that aligns with their qualifications and career goals.
- On the other hand, countries with lower unemployment benefits create a different set of dynamics. The lack of financial support forces unemployed individuals to actively search for jobs, as they may not have enough savings or assistance to survive without work for an extended period. This pressure encourages quicker re-entry into the workforce, leading to lower unemployment rates in the short term. This is the case of countries like Poland, Czechia, Hungary and Romania. Despite having lower minimum wages, they barely spent % of their GDP on unemployment social benefits and still have some of the lowest unemployment rates in Europe.  

![un_exp](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_exp.png)

**4. Economic Structure and Industry Composition**

- Spain or Greece rely heavily on tourism and hospitality, which tend to offer precarious, seasonal jobs that are vulnerable to economic downturns.
- Germany and the Netherlands, on the other hand, have strong industrial and tech sectors, which provide more stable employment opportunities.

In conclusion, the data suggests that higher minimum wages do not necessarily lead to higher unemployment. Instead, each country's economic structure, labor policies, and industry composition play a crucial role in shaping employment trends. This underscores the importance of considering broader economic factors rather than just assuming a direct link between wage growth and job losses. 

## Conclusions and Insights


## Limitations and Future Work


## References
