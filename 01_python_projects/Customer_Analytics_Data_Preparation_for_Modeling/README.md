# 🧠 Customer Analytics Mini Project  

## 📊 Project Overview  
This project focuses on **optimizing data storage and transformation** for a customer dataset to improve memory efficiency and analytical performance.  
The goal is to transform the dataset (`customer_train.csv`) into a new DataFrame named **`ds_jobs_transformed`**, using more efficient data types while filtering for specific customer profiles.  

---

## 🎯 Objectives  
- Convert categorical columns with two factors to Boolean (`bool`).  
- Store integer-only columns as 32-bit integers (`int32`).  
- Store floating-point columns as 16-bit floats (`float16`).  
- Convert nominal categorical columns to the `category` data type.  
- Convert **ordinal categorical columns** to *ordered categories* (maintaining their natural order).  
- Filter dataset to include only **students with ≥10 years of experience** at **companies with ≥1000 employees**.  

---

## 🧩 Key Features  
- Memory-optimized DataFrame construction.  
- Efficient handling of categorical and numerical data types.  
- Logical filtering for enterprise-level professional profiles.  
- Comparison of memory usage before and after transformation using `.info()` and `.memory_usage()` methods.  

---

## 🛠 Tools & Libraries Used  
- **Python**  
- **Pandas**  
- **NumPy**  
- **Jupyter Notebook**

---

## 📁 Project Files  
| File Name | Description |
|------------|-------------|
| `notebook.ipynb` | Main analysis and data transformation notebook |
| `customer_train.csv` | Original customer dataset |

---

## 🔍 Analysis Highlights  
- Performed **data type optimization** to reduce memory footprint.  
- Implemented filtering for targeted user profiles (≥10 years of experience, ≥1000-employee companies).  
- Verified transformation efficiency by comparing memory usage before and after processing.  

---

## 💡 Insights & Benefits  
- Significant reduction in **memory usage** after transformation.  
- Enhanced efficiency for **model training and analytics** workflows.  
- Clean, organized, and scalable data preprocessing structure.  

---

## 📊 Example Outputs  
After transformation:

```python
ds_jobs.info()
ds_jobs.memory_usage(deep=True)

## Output shows a substantial decrease in total memory usage compared to the original dataset.
