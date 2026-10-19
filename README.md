# FUTURE_DS_03

# MARKETING FUNNEL & CONVERSION PERFORMANCE ANALYSIS

## Future Interns – Data Science & Analytics Task 3

### 1. Executive Summary

This project analysed a bank marketing campaign dataset to evaluate customer conversion performance and identify factors associated with successful campaign outcomes. The analysis was conducted using Microsoft Power BI, with the objective of understanding how marketing contacts translate into customers, identifying major conversion and drop-off points, comparing performance across customer segments and communication channels, and providing actionable recommendations.

The dataset contained **41,188 marketing contacts**, of which **4,640 customers converted** and **36,548 did not convert**. This resulted in an overall conversion rate of approximately **11.27%**, meaning that almost nine out of every ten contacted customers did not subscribe to the product.

The analysis identified substantial differences in conversion performance across communication channels, previous campaign outcomes, customer characteristics and campaign contact frequency. Cellular communication performed considerably better than telephone communication, while customers who had previously responded positively to a marketing campaign showed a particularly high likelihood of conversion.

The findings demonstrate the importance of moving from high-volume marketing towards a more targeted and data-driven customer engagement strategy.

---

## 2. Project Objective

The main objective of this project was to analyse marketing funnel and conversion performance using customer campaign data.

The analysis aimed to answer the following questions:

- How many customers were contacted?
- How many customers converted?
- What was the overall conversion rate?
- Where are the major conversion losses occurring?
- Which communication channels perform best?
- Which customer segments have higher conversion rates?
- How does previous campaign history affect conversion?
- Does repeated customer contact improve or reduce conversion performance?
- What actions could improve future marketing campaigns?

---

## 3. Dataset Description

The analysis used the **Bank Marketing Campaign dataset**, which contains information about customers contacted during a marketing campaign.

The dataset includes demographic, financial and campaign-related variables such as:

- Age
- Occupation
- Marital status
- Education
- Housing loan status
- Personal loan status
- Contact method
- Month of contact
- Number of campaign contacts
- Previous campaign outcome
- Call duration
- Final campaign outcome

The variable **`y`** was used as the primary conversion indicator:

- `yes` = customer converted/subscribed
- `no` = customer did not convert

Because the dataset records campaign contacts rather than website traffic, it does not contain a separate website visitor stage. Therefore, the funnel analysis focuses on the measurable stages available in the dataset: **marketing contacts → converted customers**.

---

## 4. Data Preparation

The data was imported into Power BI and prepared using Power Query and DAX.

The following data preparation steps were performed:

1. Imported the Bank Marketing dataset into Power BI.
2. Checked and corrected data types.
3. Reviewed categorical variables and unknown values.
4. Retained meaningful `unknown` categories rather than unnecessarily deleting records.
5. Created a conversion indicator based on the `y` variable.
6. Created customer status categories for converted and non-converted customers.
7. Created age groups:
   - 18–25
   - 26–35
   - 36–45
   - 46–55
   - 56–65
   - 66+
8. Created DAX measures for key marketing performance indicators.

---

## 5. Key Performance Indicators

The dashboard contains four primary KPIs.

| KPI | Result |

Total Marketing Contacts | **41,188** |
Converted Customers | **4,640** |
Non-Converted Customers | **36,548** |
Overall Conversion Rate | **11.27%** |
Non-Conversion Rate | **88.73%** |

The overall conversion rate was calculated as:

**Conversion Rate = Converted Customers ÷ Total Contacts × 100**

Therefore:

**4,640 ÷ 41,188 × 100 = 11.27%**

This indicates that the campaign converted approximately one in every nine contacted customers.

---

## 6. Marketing Funnel Analysis

The campaign funnel can be represented as follows:

**41,188 Marketing Contacts**

↓  

**4,640 Converted Customers**

The conversion rate between these stages was **11.27%**, while **88.73%** of contacts did not convert.

The large difference between the number of contacts and successful conversions represents the primary opportunity for campaign optimisation.

Rather than simply increasing the number of contacts, the business should focus on identifying customers with a higher probability of conversion and using the most effective communication channels and campaign strategies.

---

## 7. Conversion by Contact Method

The analysis showed a significant difference in performance between communication channels.

| Contact Method | Approximate Conversion Rate |
|---|---:|
| Cellular | **14.74%** |
| Telephone | **5.23%** |

Cellular communication achieved a considerably higher conversion rate than telephone communication.

This suggests that communication channel selection may play an important role in campaign performance.

### Business Insight

The organisation should investigate why cellular communication performs better. Possible factors could include customer accessibility, convenience, communication preferences and timing.

However, channel performance should also be evaluated alongside campaign cost and customer volume before reallocating the entire marketing budget.

---

## 8. Conversion by Previous Campaign Outcome

Previous campaign performance was one of the strongest indicators of current conversion.

| Previous Campaign Outcome | Approximate Conversion Rate |
| Success | **65.11%** |
| Failure | **14.23%** |
| Nonexistent | **8.83%** |

Customers who had previously responded positively to a campaign had a substantially higher conversion rate than customers with no previous successful campaign outcome.

### Business Insight

Previous campaign history can therefore be used as an important lead-prioritisation variable.

Customers with a previous successful interaction could be classified as high-priority leads and targeted with personalised offers or follow-up communication.

---

## 9. Conversion by Campaign Contact Frequency

The analysis also examined the number of times customers were contacted during the current campaign.

Conversion generally declined as the number of campaign contacts increased.

For example, conversion was approximately:

- **13.04%** after one contact
- **11.46%** after two contacts
- **10.75%** after three contacts
- **9.39%** after four contacts
- **7.50%** after five contacts
- **4.25%** after eight contacts

### Business Insight

The results suggest diminishing returns from repeatedly contacting customers without changing the marketing strategy.

Continued unsuccessful contact may lead to inefficient use of marketing resources.

The organisation should consider changing the communication channel, offer or timing after several unsuccessful attempts.

---

## 10. Conversion and Call Duration

The analysis compared average call duration between converted and non-converted customers.

| Customer Outcome | Average Call Duration |
| Converted | **~553 seconds** |
| Not Converted | **~221 seconds** |

Converted customers had substantially longer average conversations.

### Business Insight

This indicates an association between customer engagement and conversion.

Longer conversations may provide sales representatives with more opportunities to understand customer needs, explain product benefits and address objections.

However, longer calls should not automatically be interpreted as causing conversion. The analysis demonstrates an association rather than a causal relationship.

---

## 11. Customer Age Group Analysis

Customer ages were grouped into the following categories:

- 18–25
- 26–35
- 36–45
- 46–55
- 56–65
- 66+

These age groups were analysed to identify differences in conversion performance.

Age segmentation allows the business to determine whether certain age groups respond more positively to the marketing campaign.

This information can be used together with other characteristics such as occupation, education and previous campaign history to develop more targeted customer segments.

---

## 12. Occupation and Customer Segmentation

Conversion rates were also compared across different occupations.

Some customer groups showed considerably higher conversion than others. For example, students and retired customers demonstrated relatively high conversion rates compared with several other occupational groups.

This indicates that customer occupation may be useful when developing targeted marketing strategies.

However, occupation should not be considered independently. Combining occupation with previous campaign outcome, communication channel and customer demographics would provide a stronger basis for customer targeting.

---

## 13. Major Drop-Off Point

The largest drop-off occurs between:

**Marketing Contact → Converted Customer**

Out of **41,188 contacts**, only **4,640 converted**.

Therefore, the primary business challenge is not generating contacts alone but improving the proportion of contacted customers who become customers.

The dashboard therefore focuses on identifying the characteristics of customers who are more likely to convert.

---

## 14. Key Findings

The analysis produced several important findings:

### Finding 1: Low overall conversion

The overall campaign conversion rate was **11.27%**, meaning that the majority of contacted customers did not convert.

### Finding 2: Cellular communication performs better

Cellular communication had an approximate conversion rate of **14.74%**, compared with **5.23%** for telephone communication.

### Finding 3: Previous campaign success is a strong indicator

Customers with a previous successful campaign outcome had an approximate conversion rate of **65.11%**, considerably higher than customers without a previous successful outcome.

### Finding 4: Repeated contacts show diminishing returns

Conversion generally declined as the number of campaign contacts increased.

### Finding 5: Customer engagement is associated with conversion

Converted customers had considerably longer average call durations than non-converted customers.

### Finding 6: Customer characteristics matter

Conversion varies across age groups, occupations, education levels and other demographic characteristics, indicating opportunities for customer segmentation.

---

## 15. Recommendations

### 15.1 Prioritise high-quality leads

Customers with a previous successful campaign outcome should receive higher priority because they demonstrate substantially stronger conversion potential.

A lead-priority model could classify customers into:

- High priority
- Medium priority
- Low priority

based on their previous campaign history and other relevant characteristics.

### 15.2 Optimise communication channels

The organisation should investigate increasing the use of higher-performing communication channels, particularly cellular communication.

However, channel decisions should also consider campaign cost, customer volume and customer preferences.

### 15.3 Reduce excessive repeated contact

Repeated unsuccessful contacts should be reviewed rather than continuing indefinitely.

After several unsuccessful attempts, the business could:

- Change the communication channel
- Change the timing
- Modify the offer
- Place the customer into a follow-up/nurturing campaign
- Temporarily stop contacting the customer

### 15.4 Use customer segmentation

Marketing campaigns should be tailored according to customer characteristics.

Potential segmentation variables include:

- Age
- Occupation
- Education
- Previous campaign outcome
- Contact method
- Loan status
- Campaign contact frequency

### 15.5 Improve customer engagement

Sales representatives should focus on understanding customer needs and addressing concerns rather than simply increasing call volume.

The relationship between call duration and conversion suggests that meaningful customer engagement may be important for successful outcomes.

### 15.6 Use historical campaign data

Previous campaign performance should be incorporated into future marketing strategies.

Customers who previously responded positively can be identified and prioritised for targeted follow-up campaigns.

---

## 16. Power BI Dashboard

The Power BI dashboard was developed to provide an interactive view of marketing performance.

The dashboard contains:

### KPI Cards

- Total Contacts
- Converted Customers
- Non-Converted Customers
- Conversion Rate

### Visualisations

- Marketing contact versus conversion
- Conversion by contact method
- Conversion by month
- Conversion by occupation
- Conversion by previous campaign outcome
- Conversion by age group
- Campaign contact frequency
- Average call duration

### Interactive Filters

- Month
- Contact method
- Occupation
- Education
- Previous campaign outcome
- Age group

These interactive features allow users to explore conversion performance across different customer segments.

---

## 17. Conclusion

The Marketing Funnel & Conversion Performance Analysis demonstrates how marketing campaign data can be transformed into actionable business insights using Power BI.

The campaign generated **41,188 customer contacts**, resulting in **4,640 conversions** and an overall conversion rate of **11.27%**. The analysis showed that conversion performance varies significantly according to communication channel, customer characteristics, previous campaign history and contact frequency.

The strongest opportunity for improvement is to move away from a purely volume-driven marketing approach and towards **targeted lead prioritisation**. Customers with previous successful campaign interactions should receive greater attention, while communication channels and repeated-contact strategies should be continuously evaluated based on their conversion performance.

Overall, the analysis demonstrates how data analytics can support marketing teams in identifying high-value customer segments, improving campaign efficiency and ultimately increasing conversion performance.
