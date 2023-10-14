## Training Machine learning project

### Project description:
The gym chain Model Fitness is developing a customer interaction strategy based on analytical data. 
One of the most common problems gyms and other services face is customer churn. Churn indicators vary from field to field.   For a gym, it makes sense to say a customer has left if they don't come for a month. Usually, if a customer joins, comes a few times, then disappears, they're unlikely to come back. In order to fight churn, Model Fitness has digitized a number of its customer profiles. 

### Goal:
To analyze customer profiles and come up with a customer retention strategy.

### Data Description:
'Churn' — the fact of churn for the month in question<br>
Current dataset fields:<br>
User data for the preceding month<br>
'gender'<br>
'Near_Location' — whether the user lives or works in the neighborhood where the gym is located<br>
'Partner' — whether the user is an employee of a partner company (the gym has partner companies whose employees get discounts; in those cases the gym stores information on customers' employers)<br>
Promo_friends — whether the user originally signed up through a "bring a friend" offer (they used a friend's promo code when paying for their first membership)<br>
'Phone' — whether the user provided their phone number<br>
'Age'<br>
'Lifetime' — the time (in months) since the customer first came to the gym<br>
Data from the log of visits and purchases and data on current membership status<br>
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
        <li>PLot feature distribution and correlation.</li>
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
        <li>PLot feature distribution by clusters.</li>
    </ol>
</ol>
