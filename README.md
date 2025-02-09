# Manufacturing Performance Analysis (Power BI)

## 1. Situation
- The Production Department is responsible for receiving production requests from the company's Planning Department. After the Purchasing Department places orders and imports raw materials into the warehouse, the production process begins.
- According to the plan, once production is completed, products will be stored in various locations to facilitate storage and distribution to customers. The production completion time may not fully align with the plan. During the process of inspecting warehouse entries, there is a possibility that goods may be damaged, and they will be rejected to ensure that only quality-assured products are stored for sale.
- Given the complexities of the manufacturing process, leaders require a dashboard to track key manufacturing metrics, enabling them to swiftly formulate strategies and make timely adjustments.

## 2. Task
-  Based on the situation and the needs given, I create an Operation Dashboard for the Production Director to provide a clear and intuitive visual overview that helps them make better decisions and operate more efficiently.  
-  Additionally, I also provide additional insights and recommendations to help optimize the production process.

## 3. Action
- I used the Design Thinking template for empathy and analysis, then selected the key metrics and dimensions for visualization. 
- I selected the tables related to Manufacturing department (connect PBI and AdventureWorks database on BigQuery)

<details><summary><strong>Design Thinking</strong></summary>
<br>
  
- Northstart metric: Total Production Cost	
- Dimension 1 - Time: StarDate, EndDate, DueDate
- Dimension 2 - Location: Name
- Dimension 3 - Product: Product Category, Sub Category, Name

![image](https://github.com/user-attachments/assets/3f09c7e8-80c1-419e-b4d9-50fd6e4f94d6)

![image](https://github.com/user-attachments/assets/3255531c-6116-41eb-9227-c16a0d6a2809)

![image](https://github.com/user-attachments/assets/bae932b4-cec8-432c-87ee-7446cd73daa5)

</details> 
<details><summary><strong>Data Processing</strong></summary>
<br>
  
1. Connect to database
2. choose table and cleaning data
3. Build schema(snowflex)

![image](https://github.com/user-attachments/assets/2a594bae-dc11-4459-8f57-41bfbb74da4e)

![image](https://github.com/user-attachments/assets/8d30cd7d-d534-48ed-8966-ad1232d18251)

![image](https://github.com/user-attachments/assets/a589a0cf-3968-4ee3-9029-28c2f76674aa)


</details> 

## 4. Result (Key insights and Recommendations)

### Key Insights

#### Overview (General Performance overview)

 ![image](https://github.com/user-attachments/assets/b64a0ff3-6778-4459-a9de-a70b96f153d7)

**Production Cost Distribution**
- Highest costs: Subassembly and Frame Forming.
→ Resources and expenses were primarily focused on these areas.  

**Monthly Production Cost Trends**  
- Costs were lower at the beginning of the year but increased from mid-year, peaking in November.  
- Yield Rate remained above 90%, except for slight drops in January, July, and December.  
→ Investigate machinery performance and production capacity during these months.  

**Production Cost Allocation**  
- 80% of costs were for components and parts manufacturing, 20% for final assembly.  
- High costs for handlebars and bike frames.  
→ Optimize production processes for these components to improve efficiency.  

 #### Production Overview

 ![image](https://github.com/user-attachments/assets/7ec218e0-70e6-45fa-940a-f06d66a2ac95)

**Production Hours Allocation**  
- Stages 6 and 7 had the highest production hours.  
→ Resources were mostly concentrated on these two stages.  

**Cost vs. Output Efficiency**  
- Stages 1 and 7 had disproportionately high production costs compared to their output.  
- Stage 1: Excessive time spent on parts and accessories, but low production output.  
→ Review process efficiency and machinery usage.  
- Stage 7: Cost variations up to 50% for Road Bikes-750, depending on size.  
→ Optimize cost allocation for different product sizes.  

**Delayed Orders Issue**  
- 56% of orders were delayed in stages 1 and 7 in July 2013.  
→ Review and adjust manufacturing workflow to reduce delays.  

### Recommendations
- The manufacturing process lacks optimization, leading to inefficiencies and high costs.  
- A comprehensive review and process adjustments are recommended.  




