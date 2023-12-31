# Home_LLC Assginment

# Bussiness Objective

**The business objective for a project focused on predicting the S&P/Case-Shiller U.S. National Home Price Index involves leveraging predictive modeling to gain insights into future trends in the housing market. The primary goal is to provide valuable information and decision support for stakeholders involved in real estate, finance, investment, and related industries. Here is a detailed business objective for the project:**

**Business Objective: Predictive Modeling for S&P/Case-Shiller U.S. National Home Price Index**

* Market Insights and Strategic Planning:

  * Objective: Develop a predictive model to forecast changes in the S&P/Case-Shiller U.S. National Home Price Index.
  * Purpose: Provide stakeholders with actionable insights into future trends in the housing market, enabling strategic planning and decision-making.

* Risk Mitigation and Investment Decision Support:
 
  * Objective: Identify potential risks and opportunities in the real estate market.
  * Purpose: Assist investors, developers, and financial institutions in making informed decisions related to real estate investments by assessing the impact of predicted home price movements.

* Financial Product Development:

  * Objective: Enhance existing financial products and create new offerings.
  * Purpose: Use predictive modeling to design financial instruments and investment products that align with anticipated changes in the S&P/Case-Shiller U.S. National Home Price Index, catering to the needs of investors and financial institutions.

* Optimizing Real Estate Portfolios:

  * Objective: Optimize real estate portfolios based on forecasted market conditions.
  * Purpose: Enable real estate portfolio managers to strategically allocate assets, minimize risks, and maximize returns by incorporating predictions of future home price movements.

* Mortgage and Loan Decision Support:

  * Objective: Assist in mortgage and loan underwriting decisions.
  * Purpose: Provide lenders with a tool to assess the potential impact of changing home prices on loan portfolios, aiding in risk management and loan approval processes.

* Policy and Regulatory Compliance:

  * Objective: Ensure compliance with regulatory requirements and industry standards.
  * Purpose: Use predictive modeling to anticipate market changes, enabling businesses to align their practices with regulatory standards and adapt to evolving market conditions.

* Enhanced Market Competitiveness:

  * Objective: Gain a competitive edge in the real estate and financial markets.
  * Purpose: Position the organization as a leader in the industry by leveraging advanced analytics and predictive modeling to offer innovative solutions and services aligned with market dynamics.

* Client Engagement and Communication:

  * Objective: Provide clients with valuable and transparent information.
  * Purpose: Enhance client engagement by delivering accurate and understandable predictions regarding the future direction of the housing market, fostering trust and long-term relationships.

# Task - Using publically available data for the national factors that impact supply and demand of homes in US, build a model to study the effect of these variables on home prices.

 * Urban population in Percentage----->urban_pop_per

*   Construction_price_index---------------->WPUSI012011
*   Employment-Population Ratio-------------->EMRATIO

*    Federal Funds Effective Rate---------->FEDFUNDS
*    GDP
*  Housing Inventory Estimate Renter Occupied Housing Units in the United States---->ERNTOCCUSQ176N	

* Housing Inventory Estimate Total Housing Units in the United States------>ETOTALUSQ176N	

*    Housing Subsidies_(Federal)------------>L312051A027NBEA

*    Median Consumer Price Index------------->MEDCPIM158SFRBCLE

*   MORTGAGE30US

* New Privately-Owned Housing Units Completed Total Units------------>COMPUTSA

*  New Privately-Owned Housing Units Under Construction----->UNDCON5MUSA

*    New Constructed_units--->COMPUTSA

*  Per Capita_GDP-------->A939RX0Q048SBEA

*  Population--------->POPTHM

*  New_Privately-Owned_Housing_Units_Under_Construction_Total_Units---->UNDCON5MUSA

* Producer_Price_Index_by_Commodity_Metals_and_Metal_Products_Iron_and_Steel-->WPU101

* Real Disposable_Personal_Income------------>DSPIC96

* S&P CASE-SHILLER Index-------------> CSUSHPISA

* Total_Construction_Spending_Total_Construction_in_the_United_States---->TTLCONS

* US population gender

* Working population--------->No_of_Persons

* Monthly_Supply_of_New_Houses_in_the_United_States-------------->MSACSR
* Total Household----->TTLHH
*  permit
*  Housing_Inventory_Estimate_Vacant_Housing_Units_in_the_United _States--->EVACANTUSQ176N

*  Median_Sales_Price_of_Houses_Sold_for_the_United_States----->MSPUS
*  Unemployment Rate ----------->UNRATE
As a proxy to the home prices, S&P CASE-SHILLER Index is used.

Most of the data is downloaded from [https://fred.stlouisfed.org/].

# Conclusion

# By obersving both shapely model we can see that features like:
* UNRATE (Unemployment Rate)
* ERNTOCCUSQ176N (Housing Inventory Estimate Renter Occupied Housing Units in the United States)
* urban_pop_per 
* Construction_price_index(WPUSI012011)
* GDP 
* M per 100 F 
* female
* male
* TTLCONS(Total_Construction_Spending_Total_Construction_in_the_United_States)
* TTLHH(Total Household)
* FEDFUNDS
* MORTGAGE30US 

**have positively impacting the variable CSUSHPISA** 
# features like: 
* A939RX0Q048SBEA(Per Capita_GDP-)
* FEDFUNDS (Federal Funds Effective Rate)
* No_of_Persons 
* Producer_Price_Index_by_Commodity_Metals_and_Metal_Products_Iron_and_Steel(WPU101) 

 **negatively impacting the variable CSUSHPISA and rest of the feautre have very less or no impact on CSUSHPISA.**

 # IN this project we are taking R2 score as evaluation metric b'coz of Simplicity of Interpretation.

 # **Though Decision tree regressor has highest R2 score but for this project we'll consider Randomforest Regressor model as final model. B'coz Randomforest is a low variance and low bias model**.
