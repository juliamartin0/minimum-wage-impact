# The Economic Impacts of Minimum Wage Increases in Europe

## Project Overview

The relationship between minimum wage increases and economic indicators like inflation, unemployment, and purchasing power parity (PPP) has been a long-standing debate among policymakers, economists, and labor advocates. In recent years, several European countries have implemented significant changes to their minimum wage policies, making it a timely issue to explore.

This project examines how changes in minimum wage levels impact three critical aspects of the economy. Specifically, the analysis focuses on answering the following research question: How do changes in minimum wage affect inflation, unemployment, and purchasing power parity across Europe?

This project combines time series analysis with visualizations in Tableau to examine data from various European countries. Some of the key questions this project addresses include:

- What trends have minimum wages followed in Europe over the past 14 years, and how have they varied across countries?
- How does the minimum wage relate to the PPP index in different countries, and how does this affect workers' real purchasing power?
- How does the relationship between minimum wage increases and inflation impact purchasing power in different countries?
- Does an increase in minimum wage lead to higher unemployment rates due to the increased cost of hiring for businesses?

The findings presented in this analysis are especially relevant for governments and organizations considering the introduction or increase of minimum wage laws, providing data-driven insights into the broader economic implications. The full data dashboard can be accessed [here](https://public.tableau.com/app/profile/julia.martin7005/viz/min_wage_project/WageDashboard#1) to explore different filters and visualize the data interactively.

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

- **Nominal Minimum Wage:** the official minimum wage set by each country in euros, standardized for consistency.
- **PPP-Adjusted Minimum Wage:** measure that adjusts the minimum wage based on purchasing power parity (PPP), allowing for fair comparisons between countries by considering differences in the cost of living. 
- **PPP Index:** a measure of how expensive a country is relative to others. A higher PPP Index means a higher cost of living, reducing the real value of wages. A lower PPP Index means the cost of living is lower, allowing wages to stretch further.

Between 2010 and 2025, minimum wages across the European countries studied have seen consistent growth, reflecting efforts to improve workers' earnings and reduce income inequality. While the rates of increase vary by country, the overall trend indicates a positive movement toward higher wages across the continent.

![min_wage_trend](https://github.com/juliamartin0/minimum-wage-impact/blob/main/min_wages_europe_2010-2025.png)

Although minimum wages have increased across Europe, the real impact on workers' purchasing power differs from country to country. While a higher nominal wage might suggest improved living standards, the cost of living plays a significant role in determining actual purchasing power. The graph below shows the relationship between PPP-adjusted minimum wages and the PPP Index for different European countries in 2023. 

![ppp_index](https://github.com/juliamartin0/minimum-wage-impact/blob/main/ppp%20index.png)

It shows that countries like Ireland, despite having high nominal wages, face a higher cost of living, which reduces the real value of those wages compared to countries with lower living costs, such as Spain or Poland. Despite these countries having much lower nominal wages, their minimum wage increases have outpaced the growth of their PPP index, giving their workers a stronger minimum wage relative to other countries.

In other words:

- A **higher PPP Index** than adjusted wages means workers' aren't keeping up with inflation or the rising costs, reducing purchasing power. As a result, workers may struggle to afford basic necessities, even if their nominal wages seem high. This scenario shows a disconnection between wage increases and the actual cost of living, causing workers' real purchasing power to be weaker than expected. In our graph, this situation applies to countries like Ireland, Lithuania, or Portugal among others.
- A **lower PPP Index** than adjusted wages, means that the cost of living in that country is relatively low compared to the increase in nominal minimum wages. This results in workers having greater purchasing power because their wages go further in terms of buying goods and services. In countries with lower living costs, workers may enjoy a higher standard of living even if their nominal wages are not as high as in other countries with higher living costs. This is the case for countries like Poland, the Netherlands, and Spain, among others.
- When the **PPP Index closely aligns with adjusted wages**, wage increases match living costs, keeping purchasing power stable and allowing workers to afford a similar amount of goods and services over time. This is the case for countries like Luxembourg and France. 

After analyzing this graph, we can conclude that **an increase in the nominal minimum wage does not always lead to an improvement in workers' purchasing power**. If inflation and cost-of-living rises faster than the wage increase, purchasing power may decline. Therefore, inflation plays a significant role in determining whether wage increases actually improve workers' purchasing power. 

## Minimum Wage and Inflation

When analyzing the relationship between minimum wage increases and inflation across European countries, we can see how wage changes impact workers' real purchasing power. While rising wages are important, their true effect depends on how they compare to inflation—both overall inflation (HICP) and inflation in essential goods like food, energy, and housing.

The graphs below show how minimum wages and inflation have evolved across countries. By examining these trends, we can assess whether wages are keeping up with inflation and how that affects purchasing power. To the right, the relationship between HICP (dotted blue line) and inflation of essential goods (blue area for electricity, green for food, orange for rent and yellow for gas).

In general:

- If **wages increase faster than HICP**, workers are more likely to maintain or improve their purchasing power. This can happen in two ways:

    i. **Wage growth is significantly higher than inflation** → This directly increases purchasing power. This is the case of Germany. As we can see in the graphs, the wage increase in 2023 was 18%, while the increase in HICP was 6%. Even though the inflation of essential goods was overall really high, the fact that wages increased so much in 2023 allowed German workers to keep a good purchasing power that year.
  
  ![germany](https://github.com/juliamartin0/minimum-wage-impact/blob/main/hicp%20germany.png)

    ii. **Even if HICP is high, essential goods inflation remains low** → Since basic necessities take up a large portion of workers' expenses, keeping their essential goods inflation lower prevents a major loss in purchasing power. This is the case for countries like Spain.
  
  ![spain](https://github.com/juliamartin0/minimum-wage-impact/blob/main/hicp%20spain.png)

- If **wages increase slower than HICP**, and **essential goods inflation (food, rent, energy) rises even higher than HICP**, workers' real incomes shrink, reducing their ability to afford goods and services. Even with nominal wage increases, the rising cost of essentials forces workers to spend a larger share of their income on necessities, effectively weakening their purchasing power. In Ireland, wage growth (7.6%) was insufficient to offset rising costs of essentials like food and rent, leading to a decline in real purchasing power.

![ireland](https://github.com/juliamartin0/minimum-wage-impact/blob/main/hicp%20ireland.png)

While these general patterns hold true in most cases, it is important to acknowledge that other economic factors can influence the relationship between minimum wage increases and purchasing power. Belgium is one of these exceptions. In 2023 it presented 2,3% of HICP while wages only increased by 0,11% and still managed to maintain a good purchasing power. The reason Belgium did not lose purchasing power is mainly due to automatic wage indexation and the sharp decline in energy prices (electricity = -27,2 %, gas = -53,8%), which offset the effects of food (14,3%) and rent (5,9%) inflation. This case highlights that while the relationship between wage increases and inflation is generally strong, exceptions exist when additional economic policies and structural factors come into play.

![belgium](https://github.com/juliamartin0/minimum-wage-impact/blob/main/hicp%20belgium.png)

Ultimately, while higher wages can protect or enhance purchasing power, they need to outpace inflation—especially in essential goods—for workers to truly benefit. It’s also worth noting that factors like tax policies, regional disparities, and economic uncertainty can influence how wage increases affect real purchasing power.

In conclusion, the real impact of minimum wage increases depends on how they compare to inflation and the cost of living, which is influenced by factors like PPP. For workers to benefit from higher wages, **wage growth must outpace inflation**, particularly in essential goods, and take into account differences in purchasing power across countries.

## Minimum Wage Increases and Unemployment Rates

One of the most debated topics in labor economics is whether increasing the minimum wage negatively affects employment levels. Traditional economic theory suggests that higher wages could lead to job losses, as higher labor costs might force businesses to cut jobs. However, data from European countries between 2010 and 2023 reveals a different trend:

- Minimum wages have steadily increased across all countries in the dataset, and, in most cases, unemployment rates have declined, showing that higher wages don't necessarily lead to higher unemployment.
- Some exceptions exist, such as Greece, which experienced a rise in unemployment around 2013 due to its financial crisis, and many countries saw temporary spikes in unemployment in 2020-2021 due to the COVID-19 pandemic.
- Countries with significant wage growth, like Lithuania and Spain, have not seen sustained unemployment increases, challenging the idea that higher wages always harm employment.

| ![unemp_spain](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_spain.png) | ![unemp_lithuania](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_lithuania.png) |
|----------------------------|----------------------------|
| ![unemp_netherlands](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_netherlands.png) | ![unemp_greece](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_greece.png) |


Despite this general trend, unemployment levels still vary significantly across countries due to structural and economic factors beyond just wage policies such as:

**1. Labor Market Flexibility**: Countries like Germany and Poland have more flexible hiring and firing policies, which help maintain lower unemployment rates. In contrast, Spain faces structurally high unemployment due to temporary contracts and rigid labor laws that make it costly to hire and fire workers.

**2. Productivity and Labor Costs**: Countries with high productivity, such as Belgium and the Netherlands, can sustain higher wages without negatively impacting employment. In lower-productivity economies, high labor costs (minimum wage + taxes + social security contributions) can discourage hiring.

**3. Unemployment Benefits and Social Protections** (*see scatter plot below*). Countries with higher unemployment benefits tend to experience higher unemployment rates. This is because workers may feel comfortable waiting for a better job opportunity or a more lucrative position, knowing they can rely on financial support for a longer period. As a result, there is less urgency to secure employment quickly, leading to a phenomenon known as "unemployment search disincentive". This situation can contribute to a temporary increase in the unemployment rate but can also offer greater economic stability for unemployed individuals. They have the financial security to take their time finding a job that aligns with their qualifications and career goals. On the other hand, countries with lower unemployment benefits create a different set of dynamics. The lack of financial support forces unemployed individuals to actively search for jobs, as they may not have enough savings or assistance to survive without work for an extended period. This pressure encourages quicker re-entry into the workforce, leading to lower unemployment rates in the short term. This is the case of countries like Poland, Czechia, Hungary and Romania. Despite having lower minimum wages, they barely spent their GDP on unemployment social benefits and still have some of the lowest unemployment rates in Europe.  

![un_exp](https://github.com/juliamartin0/minimum-wage-impact/blob/main/unemployment_exp.png)

**4. Economic Structure and Industry Composition**: The structure of an economy also plays a key role. Countries like Germany and the Netherlands, with strong industrial and tech sectors, provide more stable jobs, while Spain and Greece, reliant on tourism and seasonal work, face more vulnerability during downturns.

In conclusion, the data suggests that higher minimum wages do not necessarily result in higher unemployment. Instead, broader economic factors—such as labor market flexibility, industry composition, and unemployment benefits—play a crucial role in shaping employment outcomes. This emphasizes the need to consider these factors rather than assuming a direct link between wage increases and job losses.

## Conclusions and Insights

In conclusion, this analysis highlights that while minimum wages have steadily increased across Europe from 2010 to 2023, the effects on workers’ purchasing power and employment are shaped by a variety of factors. The relationship between wage growth, inflation, and unemployment is complex, with broader economic conditions playing a significant role in determining the real impact of minimum wage policies. The following key insights summarize the main findings of the study:

- Nominal wage increases have generally been seen across Europe, but the real impact on workers’ purchasing power varies depending on inflation and cost of living, particularly in essential goods.
- Purchasing power improvements are only realized when wage increases outpace inflation, especially in sectors like food, energy, and housing.
- Higher minimum wages do not always result in higher unemployment, challenging the traditional view that wage increases hurt job markets.
- Countries with high unemployment benefits tend to have higher unemployment rates in the short term, as workers can afford to search longer for better opportunities.
- Structural factors, such as the reliance on seasonal industries like tourism or the strength of industrial sectors, influence the relationship between minimum wages and employment trends.

These insights show that while minimum wage increases are an important tool for improving workers' income, their real impact depends on the broader economic context in which they are implemented.

## Limitations and Future Work

This analysis has a few key limitations:

- Data Availability: Not all EU countries were included due to missing data or inconsistent reporting. For example, countries like Denmark and Sweden lack minimum wage data in Eurostat, limiting the scope of the comparison.
- Data Consistency: Differences in how minimum wages are calculated across countries (e.g., number of payments per year) made direct comparisons challenging.
- External Factors: Other factors, such as political changes or economic shocks, were not accounted for but could influence the results.

Future research could:

- Include more countries by finding alternative data sources or improving data consistency.
- Standardize reporting methods to improve comparability.
- Incorporate additional economic indicators to provide a more complete analysis.
