# Credit_Risk_Modeling_Project
## The purposes of this project is:  
1. To build a Credit Risk model that predicts the Probability of Default (PD) of a customer, or, the probability that the customer will not repay their debt.
2. Create a User Interrface, to let Users input **_Informations_** of a customer, and return the **_Probability of Default_** of this customer
   - Link: https://credit-risk-pd-modeling-danny-project.streamlit.app/

![image](https://github.com/user-attachments/assets/e151fee7-316a-43c4-a10d-cb50d555112b)


**Probability of Default (PD)** is one of the concept mentioned in Basel 2, thus the next discussion will be about Basel 2 as relevant to our project.

## Basel 2 Review
**Basel 2** has 3 pillars, but **Pillar 1** is what relevant to our project.  
Pillar 1 talks about the Minimum Capital Requirement a financial institution must have, which deals with 3 types of risk
- Credit Risk - as relevant to our project
- Operational Risk
- Market Risk

![image](https://github.com/user-attachments/assets/1e58ca85-9409-4e8f-97d6-b04cc08340bb)

###  Within Credit Risk, there are 3 approaches a lending institution can take:  
1. Standardized approach (SA)
2. Foundation Internal Based Rating Approach (F-IRB)
3. Advanced Internal Based Rating Approach (A-IRB)

![image](https://github.com/user-attachments/assets/9a719055-6a7c-42be-bbd7-5ff0a1db3352)
![image](https://github.com/user-attachments/assets/b00bb55c-e72e-4e77-8a35-3e585e15034a)
![image](https://github.com/user-attachments/assets/50363918-ae23-482f-85cd-c7edbb61bcf5)

### Foundational Approach  
The amount of capital required to hold against certain assets, as mentioned in Basel 2 are the following  

**(Claim on Sovereign)**  

![image](https://github.com/user-attachments/assets/31880481-7bd8-474e-97ce-53239813a068)

**(Claim on Corporate)**

![image](https://github.com/user-attachments/assets/1a61c13e-64f4-4d7a-915b-c95c7f0fd950)

Such High capital requirement does not allow much flexibility for lenders, thus many prefer the Internal Rating Approach (IRB), which allows the use of internal data to measure **Credit Risk** more accurately and detailed, which in turn allows lenders to lend more.

### IRB approach
IRB allow banks to measure their own internal Credit Risk  

![image](https://github.com/user-attachments/assets/69b77dce-4c05-4689-bc8a-003665d0323f)

## The risk component requires to calculate are: 
- **PD - Probability of Default**
- **LGD - Loss Given Default**
- **EAD - Expossure at Default**
- **EL - Expected Loss** = **PD x LGD x EAD**

![image](https://github.com/user-attachments/assets/1fa42a0f-1718-4883-af71-f8cebca691df)

In this Project, we used Logistics Regression to Estimate the probability of default (PD)   

### Why Logistics Regression?
- Due to is interpretable nature, Logistics is prioritize.
- Also, PD Models can be used to make business decision (Application Scoring - like the website provided above) thus high level of interpretability is even more desired.
