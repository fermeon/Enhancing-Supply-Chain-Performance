# Enhancing-Supply-Chain-Performance

# Report on Plant Location Optimization for Global Manufacturing

## 1. **Introduction**
This report provides an analysis and optimization of the plant location selection for a global manufacturing company. The goal is to identify the optimal locations for manufacturing plants across five countries: the USA, Germany, Japan, Brazil, and India. The optimization considers various factors, including manufacturing variable costs, freight costs, fixed costs, and plant capacities.

## 2. **Manufacturing Variable Costs**
The manufacturing variable costs are the expenses incurred in producing each unit of the product in the respective countries. These costs were compiled from an external dataset and are critical in determining the most cost-efficient locations for production.

### **Summary of Manufacturing Variable Costs**
The variable costs across different countries are as follows:
- **USA:** $12 per unit
- **Germany:** $13 per unit
- **Japan:** $10 per unit
- **Brazil:** $8 per unit
- **India:** $5 per unit

## 3. **Freight Costs**
Freight costs are the expenses associated with transporting goods between the manufacturing plants and their respective markets. These costs vary significantly depending on the origin and destination countries, impacting the overall cost-efficiency of the supply chain.

### **Summary of Freight Costs**
Freight costs (in $/Container) between different countries are summarized below:
- **USA to Germany:** $12,250
- **Germany to Japan:** $22,750
- **Japan to Brazil:** $43,610
- **Brazil to India:** $29,750
- **India to USA:** $13,650

## 4. **Total Variable Costs**
To obtain the total variable costs, the manufacturing variable costs were combined with the freight costs. This gives a more comprehensive view of the expenses involved in producing and transporting the products.

### **Summary of Total Variable Costs**
The total variable costs, incorporating freight and manufacturing costs, for each country are detailed below:
- **USA:** $12,000 - $28,100
- **Germany:** $13,000 - $33,244
- **Japan:** $10,000 - $53,610
- **Brazil:** $8,000 - $37,750
- **India:** $5,000 - $34,400

## 5. **Fixed Costs**
Fixed costs represent the non-variable costs associated with operating a plant, such as facility rent, utilities, and administrative expenses. These costs vary by location and are crucial in the decision-making process for plant location.

### **Summary of Fixed Costs**
The fixed costs (in $/month) for each country are as follows:
- **USA:** $6,500 - $9,500
- **Germany:** $4,980 - $7,270
- **Japan:** $6,230 - $9,100
- **Brazil:** $3,230 - $4,730
- **India:** $2,110 - $6,160

## 6. **Plant Capacities**
The plant capacity is the production capability of each location, measured in thousands of units per month. Capacity constraints must be considered to meet demand while minimizing costs.

### **Summary of Plant Capacities**
The production capacities for each country are as follows:
- **USA:** 500 - 1,500 kUnits/month
- **Germany:** 500 - 1,500 kUnits/month
- **Japan:** 500 - 1,500 kUnits/month
- **Brazil:** 500 - 1,500 kUnits/month
- **India:** 500 - 3,000 kUnits/month

## 7. **Optimization Model**
An optimization model was developed using the Python library `PuLP`, which solves linear programming problems. The objective function minimizes the total cost, including manufacturing, freight, and fixed costs, subject to capacity constraints and demand requirements.

### **Decision Variables**
- **Production levels** at each plant.
- **Transportation quantities** between plants and markets.

### **Objective Function**
Minimize the total cost:
\[ \text{Total Cost} = \text{Variable Costs} + \text{Freight Costs} + \text{Fixed Costs} \]

### **Constraints**
- **Capacity Constraints:** Ensure that production does not exceed the available capacity at each plant.
- **Demand Satisfaction:** Ensure that the total production meets or exceeds the market demand.

## 8. **Results and Analysis**
The optimization results identify the most cost-effective plant locations and their respective production levels. The model helps the company make data-driven decisions about where to allocate resources and set up manufacturing plants to achieve cost savings and efficiency in the supply chain.

### **Optimal Plant Locations**
Based on the analysis, the optimal plant locations and their production capacities are as follows:
- **India:** Produces the maximum capacity due to the lowest variable and fixed costs.
- **Brazil:** Utilized for its moderate variable costs and relatively low fixed costs.
- **USA, Germany, and Japan:** Production is limited to higher-value products or where proximity to specific markets justifies the higher costs.

## 9. **Conclusion**
This report presents a comprehensive analysis of the factors influencing the location of manufacturing plants globally. The use of an optimization model provides valuable insights into minimizing total costs while meeting production and demand requirements. The findings support strategic decisions for efficient global manufacturing operations.

