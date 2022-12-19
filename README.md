# EDA-Salaries

This project is an Exploratory Data Analysis on the salaries of preofessionals working in the data domain in India.

https://github.com/aseemdandgaval/EDA-Salaries/blob/main/EDA_Industy_Salaries.ipynb <br />
(Check this notebook for a slightly in-depth explaination and the code.) 
<br>

## The Dataset

![image](https://user-images.githubusercontent.com/79587733/208517118-650829f7-5dda-45da-95e6-d5c0950abf54.png)

* The dataset contains information of the **Company Name**, **Job Title**, **Salaries Reported**, **Location** and the **Salary** of the working professional.  
* By cleaning and transformation I've added two more columns **Field** and **Level** so that more question scan be asked and inferences can be made.
* Originally  the salaries were in **Rupees(₹)**, **Pounds(£)**, **Dollars($)** , **per month** and **yearly**. They are converted into **Rupees per year(₹/yr)** for uniformity.
<br>

## Asking Important Questions
After cleaning and transforming the data, I asked some questions based on the data to get some insights. 
<br>

### **Q. Which company hires the most?**

![image](https://user-images.githubusercontent.com/79587733/208516614-7c4b4af0-42b1-4208-8956-16f654a9eb3f.png)

* Heres a list of top 10 companies that have a lot of positions
* Also based on the wordcloud, companies like Amazon, Google, IBM, Fresher, Tata Consultancy Services and more have a lot of positions in the data domain.
<br>

### **Q. What are the different sub-domains in the data industry?**

![image](https://user-images.githubusercontent.com/79587733/208516085-e457cc60-458c-4321-8f42-563084aee108.png)

* The **majority** of the the jobs are in the **Data Science** field.
* But actually resposnisbilities of Data Scientists very commonly **overlaps** some or all of the other sub domains.
* For example their work may include some data analysis and then making some machine learning models.
* It is also possible for mutiple job titles to exist for the same work, but that is not very common.
<br>

### **Q. What company pays the highest salaries and what are they?**

![image](https://user-images.githubusercontent.com/79587733/208495953-e5a579c7-7365-4395-9499-040a44da4390.png)

* The salaries are **very high** at the top level!
* The highest salary is **₹17 Crores** (17,11,48,000).
* The highest salaries are ranging from about **₹10 Crores to ₹75 Lakhs** (10,00,00,000 - 75,00,000).
* Though **only a handful of people** are making this amount of money.
* These salaries are **unusually high**, the person might be a CEO, there might be a typing mistake or the values could be fake.
* These are obviously **not an accurate represntation** of the rest.

![image](https://user-images.githubusercontent.com/79587733/208496884-e21f5f21-df7b-4d1f-b9be-3d5dfbb95928.png)

* The highest salaries are **way above the mean or median**.
* You cant even see the box plot with them included.
* The second box plot does give some insight with the highest salaries removed.
* It might be more insightful to know about the **distribution of all salaries** across a more realistic range.
<br>

### **Q. What is the distribution of salaries?**

![image](https://user-images.githubusercontent.com/79587733/208512436-4a852d81-d637-4615-a3ea-b37415f892f2.png)

* **90-95%** of people are making under **₹20 Lakhs** (20,00,000).
* You can see how the highest salaries give a **skewed represntation** of the industry, while the reality is quite different.
* Its better to class the highest salaries as the **outliers** and **remove them** when making a general inference or statement.
<br>

### **Q. What is the average and median Salaries by Fields?**

![image](https://user-images.githubusercontent.com/79587733/208513386-1097f6ea-2c58-416f-9269-17510f1ab963.png)

* Proffesionals in the **Data Science** field are making **significantly more** than people in the other domains.
* The median range from just under **₹10 lakhs - ₹5 lakhs** (10,00,000 - 5,00,000)
* Here it is **better to look at the median** yearly salary than the average.
* Because the **average is heavily affected by the outliers** inthe data, while the median is not.
<br>

### **Q. Which location pays the most salary?**

![image](https://user-images.githubusercontent.com/79587733/208514363-150f780a-4ae6-4716-a3ba-e4953c4c0ee5.png)

* Looks like **Pune**, **Bangalore** and **Hyderabad** offer higher salaries, around ₹12 lakhs (12,00,000).
* But these values are being **affected by the outliers**, so the actual average might be slightly less

![image](https://user-images.githubusercontent.com/79587733/208514886-73d5e5be-1c8a-4160-bb77-5b05968795bc.png)

<br>

### **Q. What are the salaries according to the seniority level?**

![image](https://user-images.githubusercontent.com/79587733/208515291-9199949d-208e-4969-a5f4-46896226c765.png)

* The **entry point** to jobs in the data space is around **₹6 lakhs** (6,00,00), though this might be slightly affected by the lowest yearly salaries, which were not jobs, but actually internships that paid only ₹5-10k per moth.
* If you work hard and become a **manager** or a **senior**, you can expect to earn in the range of **₹15-25 lakhs** (15,00,000 - 25,00,000).
<br>

## **Inferences and Conclusion**

* Here is the summary of the analysis done up until now:
    * There are a lot of jobs in the data industry, with companies like Amazon, Google, IBM, TCS etc. having a lot positions.
    * The general range of salaries (all levels) is about ₹6 - ₹25 Lakhs.
    * The jobs in the Data Science subdomain pay more than the other domains, while jobs in Data Analysis pay the least.
    * IT hubs like Pune, Bangalore and Hyderabad are great places to work in whith slightly higher pay than the other cites.
    * If you work hard and smartly, there is good growth in this industry with a substantial increase in pay as well.

