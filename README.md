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


## Key Findings

### Purchasing Power Parity (PPP)

One of the key questions in this analysis is whether or not an increase in the minimum wage translates into a higher real purchasing power for workers. To evaluate this, we compare:

- **Nominal minimum wage:** the official minimum wage set by each country in euros. Since some countries calculate wages over 14 payments per year, this analysis standardizes all values to a 12-payment system for consistency and comparability.
- **PPP-Adjusted Minimum Wage:** measure that adjusts the minimum wage based on purchasing power parity (PPP), allowing for fair comparisons between countries by considering differences in the cost of living. A higher PPP-adjusted wage means workers can afford more goods and services.
- **PPP Index:** a measure of how expensive a country is relative to others. A higher PPP Index means a higher cost of living, reducing the real value of wages. A lower PPP Index means the cost of living is lower, allowing wages to stretch further.

As shown in the graph below, created using Tableau, all countries in the dataset have experienced consistent increases in their minimum wage levels between 2012 and 2023. While the rates of increase have varied significantly by country, the overall pattern is clear: wages have been growing across Europe in efforts to improve workers' earnings and reduce income inequality across the continent.

![min_wage_trend](https://github.com/juliamartin0/minimum-wage-impact/blob/main/min_wage_trends.png)

This graph shows the annual increase in minimum wages in 2012, 205, and 2023 of the year-over-year growth in minimum wage rates for several European countries. This historical trend sets the stage for the analysis in this project, which investigates whether these wage increases have successfully improved the purchasing power parity (PPP) for workers in different countries.

Now that we know the wage trend has been positive and growing, let's explore whether these increases have led to better purchasing power for workers. To do this, we adjust the minimum wage using the PPP index, allowing for a fair comparison between countries.

In the graph below, we show the relationship between each country's PPP index and its minimum wage adjusted for PPP. Some interesting insights emerge. For example, having the highest nominal minimum wage doesn’t necessarily mean having the highest purchasing power. Ireland is a good example of this. Although it has one of the highest nominal minimum wages, it also has the highest PPP index (meaning the cost of living here is also very high). As a result, its minimum wage adjusted for PPP is lower than that of other high-income countries like Belgium or the Netherlands.

![ppp_index](https://github.com/juliamartin0/minimum-wage-impact/blob/main/ppp%20index.png)

This creates a gap between minimum wage and the cost of living, leaving Irish workers with less real purchasing power compared to workers in countries like Spain or Poland. Despite these countries having much lower nominal wages, their minimum wage increases have outpaced the growth of their PPP index, giving their workers a stronger minimum wage relative to other countries.

In other words:

- If the **PPP Index is higher** than the adjusted minimum wage, it means workers' wages are not keeping up with inflation or the rising prices of goods and services, leading to reduced purchasing power. As a result, workers may struggle to afford basic necessities, even if their nominal wages seem high. This scenario shows a disconnection between wage increases and the actual cost of living, causing workers' real purchasing power to be weaker than expected. This situation applies to countries like Ireland, Lithuania, Portugal, Greece, Croatia, Malta, Slovakia, Hungary, Czechia, Latvia, Estonia, and Bulgaria.
- If the **PPP Index is lower** than the adjusted minimum wage, it means that the cost of living in that country is relatively low compared to the increase in nominal minimum wages. This results in workers having greater purchasing power because their wages go further in terms of buying goods and services. In countries with lower living costs, workers may enjoy a higher standard of living even if their nominal wages are not as high as in other countries with higher living costs. This can be particularly beneficial in countries where the cost of essential goods (like housing, food, and energy) is lower, allowing workers to save more or enjoy a higher quality of life. This is the case for countries like Germany, the Netherlands, Belgium, Slovenia, Spain, Poland, and Romania.
- If the  **PPP Index closely aligns with the adjusted minimum wage**, this suggests that the increases in the nominal minimum wage have kept pace with the cost of living. This suggests that wage increases are effectively offsetting rising living costs. In these cases, workers' real purchasing power remains steady, allowing them to afford a similar amount of goods and services over time. This creates a balanced situation, which is the case for countries like Luxembourg or France. 

After analyzing this graph, we can conclude that **an increase in the nominal minimum wage does not always lead to an improvement in workers' purchasing power**. If inflation or other cost-of-living factors rise faster than the wage increase, workers may experience diminished purchasing power, even though nominal wages are higher. Therefore, inflation plays a significant role in determining whether wage increases actually improve workers' purchasing power. A higher nominal minimum wage doesn't automatically translate into better purchasing power unless it keeps pace with the cost of living and inflationary pressures within the country.

### Inflation

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

### Unemployment


## Conclusions and Insights


## Limitations and Future Work


## References
