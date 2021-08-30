# Model Card:

## Credit Line Increase Model Card: 

#### Basic information: 
* Person developing code: Youssef Ragab, yragab@gwu.edu
* Model date: August 2021
* Model version: 1.0
* License: MIT
* Model implementation code: analytics_edge_project.ipynb


#### Intended Use: 
* Primary intended use: Project for GWU DNSC 6301 bootcamp, using decision trees to predict credit line delinquency and bias remediation for protected groups.
* Primary intended users: Students of GWU DNSC 6301 bootcamp
* Out of scope use cases: Any scope beyond educational is out of scope


### Training Data 

|Name |	Modeling Role | Measurement | Level	Description |
------------------------------------------------------
|ID |	ID |	int |	unique row indentifier |
|LIMIT_BAL|	input	|float	|amount of previously awarded credit
|SEX	|demographic information|	int	|1 = male; 2 = female|
|RACE	|demographic information|	int|	1 = hispanic; 2 = black; 3 = white; 4 = asian|
|EDUCATION	|demographic information	|int|	1 = graduate school; 2 = university; 3 = high school; 4 = others|
|MARRIAGE|	demographic information|	int|	1 = married; 2 = single; 3 = others|
|AGE|	demographic information|	int|	age in years|
|PAY_0, PAY_2 - PAY_6|	inputs|	int|	history of past payment; PAY_0 = the repayment status in September, 2005; PAY_2 = the repayment status in August, 2005; ...; PAY_6 = the repayment status in April, 2005. The measurement scale for the repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; ...; 8 = payment delay for eight months; 9 = payment delay for nine months and above|
|BILL_AMT1 - BILL_AMT6|	inputs|	float|	amount of bill statement; BILL_AMNT1 = amount of bill statement in September, 2005; BILL_AMT2 = amount of bill statement in August, 2005; ...; BILL_AMT6 = amount of bill statement in April, 2005
|PAY_AMT1 - PAY_AMT6	|inputs|	float|	amount of previous payment; PAY_AMT1 = amount paid in September, 2005; PAY_AMT2 = amount paid in August, 2005; ...; PAY_AMT6 = amount paid in April, 2005|
|DELINQ_NEXT	|target|	int|	whether a customer's next payment is delinquent (late), 1 = late; 0 = on-time|




















































