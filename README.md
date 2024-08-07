# Unlocking Potential: Analyzing South African Education Practices (2023 Data)
## Insights from School and Household Surveys

![education (2)](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/e4ecbccb-58fe-497c-9a87-a15d31ec0fe9)

# 1. Overview
 
## **Problem Definition**  
The primary issue in South African public schools, particularly in township and rural areas, is **twofold**:

**1.    Lack of Specialization and Skill Development:**  
- Most schools do not specialize in areas such as electronics, programming, arts and visuals, agricultural sciences, environmental management, basic carpentry, plumbing, engineering, Woodworking, etc.
- As a result, students graduate without practical skills or the ability to leverage their talents for economic independence.
- This leads to a workforce that is unprepared for the job market, contributing to high unemployment rates and socio-economic disparities.
  
**2.    Poor Infrastructure:**
- Many schools lack basic necessities like reliable water, proper sanitation, consistent electricity, and sufficient computers with internet access. 
- This inadequate infrastructure significantly hampers effective teaching and learning.
- Students struggle to access information, utilize online resources, and develop the crucial 21st-century skills needed for the 4th Industrial Revolution (4IR) – skills that are fundamental for success in today's job market. This widens the skills gap and restricts students' future opportunities.

## **Objectives**  
  
**1. Highlight the Importance and Urgency:** 
- Use data to underscore the critical need for specialized education and improved infrastructure in South African public schools.

**2. Provide Actionable Insights:**
- Offer data-driven recommendations for decision-makers to prioritize interventions and allocate resources effectively.
- Suggest strategies to transition schools towards specialized education and improve overall infrastructure.

## **Motivation**
Many schools in my community lack specialization in crucial fields, leaving our graduates unprepared for the job market. This reality hits close to home, as I see talented students around me struggle to find their footing, contributing to high unemployment rates and socio-economic disparities. I urgently want to conduct a data analysis project to understand and address these gaps, so we can recommend actionable solutions that equip our youth with valuable skills, reduce unemployment, and foster a thriving, self-sufficient community.

## **Insights**  

**Critical Need for Specialized Education and Improved Infrastructure in South African Public Schools**

The data presented highlights the crucial need for specialized education and improved infrastructure in South African public schools. Here's a closer look at the evidence:

### **1. Mismatch Between Skills and Regional Needs:**

**High Number of Ordinary Schools:**
- Provinces like **KwaZulu-Natal** and **Eastern Cape** have the most ordinary schools. While foundational education is essential, it doesn't necessarily equip students with skills directly relevant to the regional economy.
  
**Uneven Distribution of Specialized Schools:**
- **Eastern Cape** leads in agricultural and technical schools, aligning with its economic activities. However, the picture is less clear for other provinces. **Mpumalanga** has the most full-service and Dinaledi schools (purpose unclear), while **Western Cape** has the most schools with unknown specializations. This indicates a lack of focus on specific industries in some regions and potential data collection issues.

### **2. High Unemployment Rates:**
  
- **Mpumalanga** (41%) and **KwaZulu-Natal** with a heavy reliance on grants, show the highest unemployment rates. This suggests a skills gap between the education system's output and the needs of the labor market.  
  
### **3. The Digital Divide:**
  
- **Gauteng** boasts the highest internet access (36.24%) and laptop ownership (37.88%), while **Eastern Cape** (1.15% & 14.45%) and **Limpopo** (0.74% & 17.54%) have the lowest. This digital divide hinders access to information, online learning resources, and **21st-century skills development**, crucial for employability in the modern world.

### **4. Learner-Educator Ratios:**

- **Gauteng** has the highest learner-to-educator ratio. While this could be due to **larger schools**, it can also indicate **overcrowded classrooms** and potentially less individualized attention for students.

     
# 2. Data Understanding and Preparation  
This section details the process of transforming raw data from multiple sources into a clean and structured format ready for analysis.  
###  **2.1 Data Collection**  
Data for this project was sourced from two primary datasets:
1.	**ECD Masterlist Data, Quarter 3 of 2023 (Department of Basic Education, South Africa)**  
 	- **Source:** Official government website (https://www.education.gov.za/Programmes/EMIS/EMISDownloads.aspx.).  
 	- **Processing:**  
      - Removed unnecessary details such as IDs, payroll data, specific location data, historical information, and unclear fields.  
      - Retained essential data including school identification, location (province, city, etc.), type, status, and enrollment information (learners, educators).

2.	**General Household Survey 2022 (Statistics South Africa)**  
	- **Source:** SuperWEB2 platform (https://superweb.statssa.gov.za/webapi/jsf/login.xhtml).  
	- **Processing:**  
   	   - Condensed age group data from specific ranges (e.g., 05-09, 10-14, 15-19, 20-24 years) into broader categories (e.g., 05-24 years) for enhanced analysis.  
	    
**2.2 Data Cleaning**  
Initial data cleaning was performed in Microsoft Excel to ensure consistency and accuracy. Key steps included:  
   - Converting downloaded data from CSV to Excel format.  
   - Removing irrelevant columns to streamline the dataset.  
   - Using Power Query Editor to merge related sheets for improved organization.  

**2.3 Advanced Cleaning**
The advanced data cleaning stage involved more sophisticated techniques to further refine the datasets, ensuring they were ready for in-depth analysis. This stage included:
- **Standardizing Data Formats:** Ensured uniformity in date formats, text cases, and numerical precision.
- **Handling Missing Values:** Applied imputation methods and, where necessary, removed rows or columns with excessive missing data.
  
**2.4 Data Integration**
Data from the two primary sources were integrated to create a comprehensive dataset. This involved:
- **Consolidation of Datasets:** Combined datasets to form a unified dataset, ensuring that all necessary variables were included and correctly aligned.
  
**2.5 Data Validation**
The final dataset was subjected to rigorous validation checks to ensure its reliability and accuracy:  
- **Consistency Checks:** Verified that data was consistent across different sources and formats.   
- **Accuracy Verification:** Cross-checked a sample of the data against original sources to ensure accuracy.  
- **Completeness Assessment:** Ensured that the dataset was complete with no missing critical information.  
  
**Tools Used:** Web Browsers, Python (pandas, NumPy), Microsoft Excel
  
By meticulously preparing the data through these stages, I ensured a robust foundation for subsequent analysis, enabling accurate and meaningful insights to be drawn from the data.

# 3. Exploratory Data Analysis (EDA)

**3.1 Descriptive Statistics:**  
Provide a summary of key variables to understand their distribution and central tendencies.  
  
**3.2 Analysis of Specialization and Skill Development:**  
Examine trends and patterns in specialization and skill development across different segments.  
  
**3.3 Analysis of Infrastructure:**  
Identify regions with the most critical infrastructural needs.  
  
**3.4 Correlation Analysis:**  
Explore relationships between variables, such as Economic Quintile and Specialization, and the number of Learners versus Educators.  
  
**3.5 Comparative Analysis:**  
Conduct comparative analyses to draw meaningful insights.  
  
Used charts and graphs to visualize data, facilitating the identification of patterns and trends.


## **Summary**  
  
Our exploratory data analysis focused on South African public schools, particularly in urban and rural areas.

**Findings include:**

### 1. **Learner and Educator Distribution:**

- **Significant variation** in the number of learners (0 to 3,233) and educators (0 to 372) per school, with **average** counts of 542 learners and 19 educators **(28:1)**, respectively.

![School Size Distribution (Learners and Educators)](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/69a04d4a-4a36-471b-85aa-5665b928f827)
School Size Distribution (Learners and Educators)


### 2. **School Distribution:**

- The data suggests a potential **imbalance** in school distribution, with a **higher** concentration in lower economic quintiles (Q1 & Q2) compared to wealthier ones (Q4 & Q5).
- Availability of specialized schools (technical, comprehensive) appears **limited**, potentially restricting access to diverse career paths.

  ![Economic Quintile vs  Specialization](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/cbd1bb93-fe64-4734-9792-6c4a478a07e5)
Economic Quintile vs. Specialization


### 3.  **Population Across Provinces:**

- **Average** provincial population is 6,820,463, with considerable **variation** (1,294,044 to 16,266,595).

![Regional Population Distribution](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/1d0326e3-a9e0-4cd0-9893-c698451f183a)


### 4. **Income Sources:**

- **Salaries/wages/commission** are the primary income source (51%), followed by **grants** (30%).

![Income Source Composition](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/4c901228-0897-4c40-9bcd-8030ab334bbe)


### 5. **Employment Status:**

- **Wide** regional disparities in employment, with **averages** of 1,941,827 **employed**, 997,709 **unemployed**, and 1,930,693 **not economically** active individuals.

### 6. **Educational Attainment:**

- **High completion rate** of **Grade 12 - Standard 10 - NQF4**, but steep **decline** in **higher education** attainment.

![Highest Education Level](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/a6356e29-efaf-4fa5-99c9-b6303b79d9a6)


### 7. **Infrastructure Access:**

- **Significant digital divide**, with urban areas having much higher access to internet libraries, desktops/laptops, and electricity compared to traditional and farm settings.
  
![Infrastructure Access by Geography Type](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/f8ce0ffd-b072-4f2b-ae40-c742ee43803a)

### 8. **Commute Times:**

- **Most students** commute **within 31-60 minutes**, with **urban areas** showing a **broader range** of commute durations.

  ![Time Taken to School by Geography Type](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/dda4de97-8ca3-4bbe-9fc8-133811a399a7)


## **4. In-Depth Analysis**  

### **4.1 Lack of Specialization and Skill Development**

#### (i) Provincial Population Breakdown by Age Group 
- The chart reveals a youthful population concentrated in Limpopo and Mpumalanga, while Western Cape and Gauteng hold the largest working-age populations, potentially impacting future education needs and workforce distribution.

![Provincial Population Breakdown by Age Group](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/6dbb9928-29db-4e2e-b181-41299c22cf71)


#### (ii) Visualizing Specialization Distribution Across Provinces  
- The distribution of schools in South Africa highlights a focus on basic education in KZN and EC, while NW and EC prioritize comprehensive and specialized education potentially aligned with regional economic needs.
  
![Specialization Distribution Across Provinces](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/2f7e33e4-beb4-4769-aea7-852341586a90)


#### (iii) Household Income in Provinces: Population Distribution by Main Source  
- Gauteng and Western Cape lead in formal employment, while Eastern Cape, KwaZulu-Natal, and Limpopo show a higher reliance on government grants.
- Mpumalanga and Northern Cape have more balanced income sources, with significant contributions from business activities and farming in the latter.

![Population Distribution by Main Source](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/773a9d9f-24a1-434a-a98f-4c055005b308)

    
#### (iv) Understanding South Africa's Unemployment Landscape by Province  
- Unemployment rates vary significantly across provinces, with Mpumalanga, KwaZulu-Natal, Eastern Cape, and North West exceeding 30%, while Western Cape fares better.
- Mpumalanga faces the most concerning situation with an unemployment rate of 41%, whereas Western Cape enjoys the lowest rate at 21%
  
![Unemployment Landscape by Province](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/bb523c51-cf24-456c-a0d1-bbdcb122c46b)


### **4.2 Infrastructure**  

#### (i) Provincial Breakdown: Urban vs. Rural Schools  
- While KZN, Eastern Cape, and Limpopo have more schools in rural areas, Gauteng, Free State, and Western Cape likely have a higher concentration in urban areas. Data is missing for Mpumalanga and North West.
  
![Urban vs  Rural Distribution](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/a86d55da-22c7-4d3c-a210-d243e5b1d407)


#### (ii) Provincial Breakdown: Learners, Educators, and Schools (Percentage)
- The distribution of schools and educators varies across provinces, with Gauteng having larger, more populated schools and KwaZulu-Natal boasting a wider network of smaller schools. Learner-to-educator ratios suggest potential overcrowding in Gauteng and a more balanced distribution in Western Cape.

![Learners, Educators, and Schools (Percentage)](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/ddffc6cb-34ff-4b5f-888e-d58bbf258041)

#### (iii) Distance and Education Access: A Look at Urban vs. Rural Student Travel Times  
- Urban students tend to have shorter commutes compared to rural students, with Gauteng boasting the highest percentage of students with commutes under 30 minutes. While long commutes are uncommon overall, rural areas see a higher prevalence of moderate commutes (30-60 minutes).
  
- This suggests location plays a significant role in student travel times, potentially impacting access to education in some rural areas.
  
![Urban vs  Rural Student Travel Times](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/a64948db-07d5-45b4-b797-a0e721ccf8e1)



#### (iv) Understanding Provincial Variations in Infrastructure Availability  
- Vast disparities exist between provinces in internet access (highest: Gauteng, lowest: Eastern Cape) and laptop ownership (highest: Western Cape, lowest: Mpumalanga). Electricity access is more uniform, but still uneven (highest: Gauteng, lowest: Eastern Cape).
  
![Provincial Variations in Infrastructure Availability](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/94ae215d-4564-480d-bd1e-d6975b93a3bf)

![Provincial Deficits in Basic Infrastructure Access](https://github.com/DesmondMokhali/National_School_Analysis/assets/121891418/db1d6600-ffb5-4748-a634-58693bb840f3)


## **5. Conclusion**  

The analysis highlights significant gaps in the South African public education system, particularly in township and rural areas. The lack of specialization and inadequate infrastructure are key factors contributing to high unemployment rates and socio-economic disparities. Without practical skills and a supportive learning environment, students struggle to compete in the job market and leverage opportunities for economic independence. Addressing these issues is crucial for equipping the youth with the skills needed for the 4th Industrial Revolution and fostering a thriving, self-sufficient community.
     
## **6. Recommendations:**

### 1. Develop Specialized Education Programs:
  
**Curriculum Enhancement:**
- Introduce specialized courses in electronics, programming, arts, agricultural sciences, environmental management, carpentry, plumbing, engineering, and woodworking.

**Teacher Training:**
- Invest in professional development for educators to ensure they can effectively teach specialized subjects.
- Partnerships with Industry: Collaborate with local businesses and industries to provide practical training and internship opportunities for students.

  
### **2. Improve School Infrastructure:**
  
**Basic Necessities:** Ensure all schools have reliable water, proper sanitation, consistent electricity, and sufficient computers with internet access.

  
**Modern Learning Environments:** Upgrade facilities to support modern teaching methods and technologies, including well-equipped science and computer labs.
  
**Maintenance and Sustainability:** Implement regular maintenance schedules and sustainable practices to keep infrastructure in good condition.

### **3. Address the Digital Divide:**

**Technology Access:** Provide students with access to laptops and internet connectivity to support online learning and research.
  
**Digital Literacy Programs:** Integrate digital literacy into the curriculum to equip students with essential 21st-century skills.
  
**Community Wi-Fi Hubs:** Establish community centers with internet access where students can study and complete assignments.

### **4. Align Education with Regional Needs:**
  
**Economic Relevance:** Tailor educational programs to meet the specific economic needs of each region, ensuring students gain skills that are in demand locally.
   
**Data-Driven Decisions:** Use data to identify and address gaps in the current education system, prioritizing interventions where they are most needed.
  
**Continuous Monitoring and Evaluation:** Implement a robust monitoring and evaluation framework to track the progress and impact of educational initiatives.

## **7. Future Work:** 

**Title:** School Infrastructure Mapping Project

**Vision:** To create a comprehensive and interactive map of South African schools, highlighting infrastructure needs and opportunities for specialized programs.
  
### **Mission:**
- Gather data on current school infrastructure through community input.
- Identify areas requiring focused support in areas like electronics, programming, arts, and agricultural sciences.
- Empower stakeholders to contribute to shaping the future of South African education.

### **Next Steps:**
  
**Community Input:** Teachers, principals, learners, parents, and community members can use dedicated Forms to share information about their schools.
  
**Data Collection:** These contributions will be used to map out the current state of school infrastructure and identify areas needing specialized programs in fields like electronics, programming, arts, agricultural sciences, and more.
    
**Geospatial Analysis and Maps:** We will utilize geospatial analysis to create detailed maps that visualize school conditions across different regions.
   
**Data Analysis and Predictive Analytics:** Data analysis and predictive analytics will be applied to identify trends and forecast future needs for infrastructure and specialized programs.
   
**Data Pipelines and Databases:** To manage and process the collected information efficiently, we will implement robust data pipelines and databases.
   
**Interactive Dashboards:** Interactive dashboards will be developed to present data insights and allow users to explore the information dynamically.


### **Why Contribute?**  

**Empower Change:** Provide valuable insights that will directly influence improvements in school infrastructure and specialized education programs.
     
**Foster Collaboration:** Work together with others to create better educational facilities and opportunities for all students.
    
**Make a Difference:** Shape the future of South African education by providing impactful data.
    
**Create a Better Learning Environment:** Together, we can build a brighter future for our schools with improved infrastructure and specialized programs.


### **The ARC Platform**

We are building the Academic Resource Center (ARC), a platform specifically designed to house and analyze data from the School Infrastructure Mapping Project. ARC will feature user-friendly, interactive dashboards that provide real-time insights into school conditions, infrastructure needs, and areas where specialized programs would be most beneficial. This platform will be central to our efforts in improving education by offering a comprehensive view and actionable data for policymakers, educators, and communities.
    

![ARC](https://github.com/user-attachments/assets/df24ce86-5571-41c0-8ef0-730655be615e)


![ARC Cont](https://github.com/user-attachments/assets/4200b659-fb57-4abe-b1be-f057150d2ff4)




