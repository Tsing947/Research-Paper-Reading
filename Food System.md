Created by Huatsing on 26 Jul 2024
# Food System related paper
## Optimization
### Province-specific sustainable diets in China considering nutrition, environment, affordability, and acceptability
***Journal of Clearner Production 2024***  
**Cheng Guangyan and Liu Gang; Wang Huijun (疾控中心** 
* Aim  
In this study, we aimed to address the abovementioned research gap by optimizing food consumption in Chinese provinces from all these ***nutritional, environmental, economic, and cultural*** (i.e., acceptability with the minimum changes) perspectives adopted the ***non-linear programming approach*** to identify sustainable diets for 31 provinces in mainland China.
* Data  
15种类 including cereals, tubers, legumes, vegetables, fruits, nuts, pork, beef, mutton, poultry, eggs, dairy products, fish and seafood, sugar, and oil. Due to lack of data on salt intake, we assumed a salt intake of 5 g for all provinces with no further optimization  
*away from home*, ***CHNS 2018***  
按照弹性系数比重进行估算比例 方法同《2021中国与全球食物政策报告》正式发布(附全文) https://agfep.cau.edu.cn/art/2021/4/30/art_39027_744843.html 附录2提供了弹性系数，以及计算的2012-2019的在外就餐消费比例  
$F_{ij} = \frac{h_{ij}}{(1 - r_i \cdot (1 + e_i \cdot \frac{(I_j - \bar{I})}{\bar{I}}))}$  
where Fij denotes the consumption of food item i in province j;  hij denotes the consumption; ri denotes the average proportion of out-of-home consumption in the CHNS 2018 survey provinces; ei denotes the income elasticity of the out-of-home consumption of ; Ij denotes the average income of residents; and Idenotes the average income of the CHNS 2018 survey provinces.   
*Evinronmental Footprint*: recently Chinese available (Cai et al., 2022; Xue et al., 2021) environmental footprint factors, i.e., carbon footprint (CF), water footprint (WF), land footprint (LF), nitrogen footprint (NF), and phosphorus footprint (PF) per gram of food to all food items. 这是目前最全面的针对中国的食物环境足迹数据  
*Nutrition intake*: Chinese Food Composition Tables (Yang, 2019a, 2019b)
four essential nutrients (vitamin K, vitamin B-6, vitamin B-12, and saturated fatty acids) were not available in the Chinese food composition table, complemented the nutrient composition datasets with the nutrient content values for these nutrients from the United States Department of Agriculture (USDA) Standard Reference (SR) 28 nutrient composition table.  
Obtained the daily per capita intake of calories and 24 essential nutrients (20 beneficial and 4 restricted) for the 31 provinces.
$MNA = \frac{1}{21} \sum_{n=1}^{21} \frac{QN_n}{RNI_n}$  
$MNA = \frac{1}{4} \sum_{n=1}^{4} \frac{QN_m}{UL_m}-1$  
常用的一种计算方法，分别计算 we used the mean nutrient adequacy (MNA) ratio, recommended nutrient intakes (RNIs) of calories and beneficial nutrients and restricted nutrients MNE (saturated fatty acids, cholesterol, Na and sugar)
*Agricultural price data* each province from the China Agricultural Products Supply and Demand Analysis System of the Ministry of Agriculture and Rural Affairs (https://ncpscxx.moa.gov.cn/) and the Agricultural Products Business Information Public Service Platform (http://nc.mofcom.gov.cn/). The data included the weekly price data for grains, tubers, legumes, vegetables, fruits, pork, beef, mutton, poultry, eggs, fish and seafood, nuts, and edible oil for each province. Owing to the lack of the price data for milk and sugar in each province, the prices of milk and sugar were replaced by the national average retail price.  
* Optimazitaion function
*Objectiive function*偏好最小  
$\text{Minimize} \ f = \frac{1}{15} \sum_{i=1}^{15} \left( \frac{Q_{\text{opt},i} - Q_{\text{obs},i}}{Q_{\text{obs},i}} \right)^2$
*Constraint*考虑了健康，环境外，还考虑了价格因素这是以往很少考虑的
$\sum_{i=1}^{15} Q_{\text{opt},i} * \text{Nutrient}_{i,n} > RNI_n$
$\sum_{i=1}^{15} Q_{\text{opt},i} * \text{Nutrient}_{i,m} < UL_m$
$\sum_{i=1}^{15} P_i * Q_{\text{opt},i} \leq \sum_{i=1}^{15} P_i * Q_{\text{obs},i}$
$\sum_{i=1}^{15} CF_i * Q_{\text{opt},i} = \alpha \sum_{i=1}^{15} CF_i * Q_{\text{obs},i}$
$\sum_{i=1}^{15} WF_i * Q_{\text{opt},i} \leq \sum_{i=1}^{15} WF_i * Q_{\text{obs},i}$
$\sum_{i=1}^{15} LF_i * Q_{\text{opt},i} \leq \sum_{i=1}^{15} LF_i * Q_{\text{obs},i}$
$\sum_{i=1}^{15} NF_i * Q_{\text{opt},i} \leq \sum_{i=1}^{15} NF_i * Q_{\text{obs},i}$
$\sum_{i=1}^{15} PF_i * Q_{\text{opt},i} \leq \sum_{i=1}^{15} PF_i * Q_{\text{obs},i}$



  
### Optimization of residents' dietary structure with consideration of greenhouse gas mitigation and nutritional requirements
***Sustainable Food production and Consumption***  
***Su MeiRong***  
Unreading

- [ ] 整理朱媛媛膳食指南对比的表格
- [ ] Food Losses and Food Waste in China https://www.oecd-ilibrary.org/content/paper/5jz5sq5173lq-en

