## Training Machine learning project

### Project description:
The gym chain Model Fitness is developing a customer interaction strategy based on analytical data. 
One of the most common problems gyms and other services face is customer churn. Churn indicators vary from field to field.   For a gym, it makes sense to say a customer has left if they don't come for a month. Usually, if a customer joins, comes a few times, then disappears, they're unlikely to come back. In order to fight churn, Model Fitness has digitized a number of its customer profiles. 

### Goal:
To analyze customer profiles and come up with a customer retention strategy.

### Data Description:
'Churn' — the fact of churn for the month in question<br>
#### Current dataset fields
#### User data for the preceding month
'gender'<br>
'Near_Location' — whether the user lives or works in the neighborhood where the gym is located<br>
'Partner' — whether the user is an employee of a partner company (the gym has partner companies whose employees get discounts; in those cases the gym stores information on customers' employers)<br>
Promo_friends — whether the user originally signed up through a "bring a friend" offer (they used a friend's promo code when paying for their first membership)<br>
'Phone' — whether the user provided their phone number<br>
'Age'<br>
'Lifetime' — the time (in months) since the customer first came to the gym<br>
#### Data from the log of visits and purchases and data on current membership status
'Contract_period' — 1 month, 3 months, 6 months, or 1 year<br>
'Month_to_end_contract' — the months remaining until the contract expires<br>
'Group_visits' — whether the user takes part in group sessions<br>
'Avg_class_frequency_total' — average frequency of visits per week over the customer's lifetime<br>
'Avg_class_frequency_current_month' — average frequency of visits per week over the preceding month<br>
'Avg_additional_charges_total' — the total amount of money spent on other gym services: cafe, athletic goods, cosmetics, massages, etc.<br>

### Plan:
<ol>
  <li>Open and preprocess the file.</li>
  <li>Study the data.</li>
    <ol>
        <li>Find mean and std of all features.</li>
        <li>Find mean and std of all features grouped by churn value.</li>
        <li>Plot feature distribution and correlation.</li>
    </ol>
  <li>Build a Binary classification model (Logistic Regression and Random Forest).</li>
    <ol>
        <li>Divide the data.</li>
        <li>Find precision/accuracy/recall.</li>
    </ol>    
  <li>Create user clusters with K-means clusterization.</li>
    <ol>
        <li>Plot a dendrogram.</li>
        <li>Train and test the clustering model.</li>
        <li>Plot feature distribution by clusters.</li>
    </ol>
</ol>

### Examples of graphs:

![image](https://github.com/gzhuldas/Training_Machine_learning_project/assets/72769986/25bbb996-8837-4224-ae17-528c2ca2aea0)


![image](https://github.com/gzhuldas/Training_Machine_learning_project/assets/72769986/b6097564-f0d1-4852-9f76-70d8a5f4d7f1)


![image](https://github.com/gzhuldas/Training_Machine_learning_project/assets/72769986/464c2e87-738a-4080-acb5-5e919143ed74)


### Conclusion:
Churn groups have similarities:Most users leave their phone numbers. People live near the gym and there are almost the same number of men and women. Clients who stay buy more additional stuff, usually have a longer contract period, prefer to attend the gym with partners 2 times a week on average. 60% of clients who stop attending classes are single, whereas only 45% of clients who stay indicated that they are single.<br>The clusters definitely differ in terms of churn rate. The 1, 4, 2 clusters are at the highest risk of leaving the classes, whereas 0, 1 are ~98% and ~91% likely to stay, respectively. The 0 cluster has the lowest churn rate, clients from this cluster are likely to attend the gym with their partners, they prefer group visits more than other and sign up for the longest contract period. All clusters have approximately the same mean age. The 1st and 4th clusters have the highest churn rate, clients from these groups are not likely to bring their partners, they spend less hours at gym per week and sign up for the shortest contract period.<br>A portrait of a loyal customer - he/she has a partner and wants to attend the gym with a partner or train in groups, is around 30 years old, lives nearby, signs up for a long period, is interested in sport products and attends the gym consistently 3-4 times a week. Based on that marketers should focus their attention on creating a family friendly atmosphere, maybe offer a deal for people who have kids as the target audience is 28+ couples.<br>As was said above an important observation from the analysis is that people who do not stop gym classes usually go there with partners or attend group sessions. On contrary, people who are most likely to discontinue the sessions do not attend group trainings and come alone. This may mean that other people (partners/personal trainers/groupmates) motivate a client to stay. So one recommendation for the gym is to offer loners to attend group trainings or come with a friend or a partner.



