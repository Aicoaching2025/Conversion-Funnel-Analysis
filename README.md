# 🚀 **Cool T-Shirts Inc. Conversion Funnel Analysis** 👕💰


## **📌 Overview**
This project analyzes the conversion funnel of **Cool T-Shirts Inc.** to understand user behavior from visiting the website to making a purchase. The analysis helps identify drop-off points and opportunities for improving conversion rates.

## **🎯 Goals**
✅ Understand how users move through the sales funnel.  
✅ Identify where users drop off at each stage.  
✅ Calculate the average time taken from visit to purchase.  
✅ Recommend improvements to enhance the shopping experience.  

## **📂 Dataset**
The analysis is based on four datasets:
📌 **visits.csv** – Users who visited the website.  
🛒 **cart.csv** – Users who added a t-shirt to their cart.  
💳 **checkout.csv** – Users who started the checkout process.  
🎉 **purchase.csv** – Users who completed the purchase.  

Each dataset contains a `user_id` and a timestamp indicating when the action occurred.

## **🔎 Project Steps**
### **1️⃣ Data Inspection**
- 🔍 Print the first few rows using `head()`.
- 🏗️ Check the structure and missing values.

### **2️⃣ Merging DataFrames**
- 🔗 Perform **left merges** to combine `visits` → `cart` → `checkout` → `purchase`.
- 📊 Store the final merged dataset in `all_data`.

### **3️⃣ Conversion Rate Analysis**
📉 Calculate the percentage of users who:
- 🏃 Visited but didn’t add an item to the cart.
- 🛍️ Added an item to the cart but didn’t proceed to checkout.
- 💳 Started checkout but didn’t complete the purchase.
- ❌ Identify the weakest step with the highest drop-off rate.

### **4️⃣ Average Time to Purchase**
⏳ Compute the time difference between `visit_time` and `purchase_time`.  
📆 Calculate the average time taken to complete a purchase.  

## **📊 Key Findings**
📌 **Drop-off points**: The highest drop-off occurs at the cart stage.  
⏱️ **Time to purchase**: The average time from visit to purchase is **~43 minutes**.  
💡 **Potential Improvements**:
- 🛒 **Reduce cart abandonment** by offering incentives.
- 🔄 **Improve checkout process** with fewer steps.
- 📩 **Send reminders** to users who added items but didn’t buy.

## **⚙️ Installation & Usage**
1️⃣ Clone the repository:
   ```sh
   git clone https://github.com/yourusername/cool-tshirts-funnel.git
   cd cool-tshirts-funnel
   ```
2️⃣ Install dependencies:
   ```sh
   pip install pandas numpy matplotlib seaborn
   ```
3️⃣ Run the analysis:
   ```python
   python funnel_analysis.py
   ```

## **👨‍💻 Author**
- **Your Name**  
- 🔗 **LinkedIn**: [Your LinkedIn](https://www.linkedin.com/in/yourprofile/)  
- 🐙 **GitHub**: [Your GitHub](https://github.com/yourusername/)  

## **📜 License**
This project is licensed under the **MIT License**.
