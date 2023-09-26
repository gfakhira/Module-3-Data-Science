# Module-3-Data-Science
## **Travel Insurance**

## **Context**

Travel insurance is a type of insurance that provides protection as long as we travel both domestically and abroad. Several countries have even required travelers to have travel insurance, for example, countries in Europe and America. The amount of premium depends on the coverage desired, the length of the trip, and the purpose of the trip. A company engaged in travel insurance wants to know the policyholder who will submit an insurance claim for coverage. Policy holder data at insurance companies is historical data consisting of destinations, insurance products, and so on.

## **Business Problem**

Insurance Company wanted to know the prediction of possible customers that made Insurence Claim for Travel Insurance. Therefore, they hired Data manpower for creating Machine Learning and used Machine Learning to made a prediction of of Travel Insurance Claim. 

For example, If customers purchase a **basic travel insurance policy** that includes trip cancellation coverage, you can expect to pay between 5% and 10% of your trip costs. For instance, if you buy a **$10,000, nine-day trip** through the Greek Isles, you can expect to pay **between $500 and $1,000**. Let's just say Customer will get maximum amount paid $1,000. The passage also mentions that adding **"Cancel for Any Reason"** coverage to your policy can increase the cost by an **additional 40% to 60%**. This type of coverage allows you to cancel your trip for any reason and receive a refund for most of your prepaid, non-refundable expenses.

We can make an assumption that for **1 Person** took **Basic Travel Insurance** with Maximum amount to be paid for taking Insurance Policy is **$1,000** as deposit amount with **"Cancel for Any Reason"** at rate of **additional cost of 40%** The Total Amount is :

- 1,000 + 40% = 1,000 + 400 = **$1,400** 

- Let's say that if the Costumers asked for Claim with **"Cancel for Any Reason"** means Company must give the Policy Amount with Deposit and Additional Cost at **$ 1,400** 
- If the Customer is Not Claim (**Without "Cancel for Any Reason"**) means Company must give the Policy Amount **Only** for the Insurance **Coverage without Deposit** at **$ 400** 

<br>

**1. False Negative**

When Customer Predicted Not Claim but in actual is Claimed with **"Cancel for Any Reason"**. In this case insurance company will need to provide the amount of insurance policy according to travel package assigned by customer. Company must pay the Policy Amount the Costumers Claim with Deposit and Additional Cost at **$ 1,400** 


**2. False Positive**

Where Customer predicted Claim but actully Not Claim, **Without "Cancel for Any Reason"**. In this case insurance company will need to provide the amount of insurance policy according to travel package assigned by customer. Company must give the Policy Amount only for the Insurance Coverage without Deposit at **$ 400** 

<br>

Reference:
https://www.forbes.com/advisor/travel-insurance/trip-cancellation/ 


## **Insight**

In this project, I tried to **Predict the Claim** for Travel Insurance made by customers. Based on statement above, **Recall** Metric is used in order to **Minimize the False Negative**. Letter on found out that the dataset had an **Extreme Imbalance data**. By finding Best algorith as Best Base Model for **Model Benchmark, Hyperparameter Tuning, and Maximizing Threshold** were took as one of steps needed to improve the model, with efforts made to handle imbalance data through techniques like **SMOTE, NearMiss, RandomOverSampler, and RandomUnderSampler** during hyperparameter tuning. It is a significant challenge to deal with it in order to Avoid Biased Output (Classifying all the target in 1 category only).  

