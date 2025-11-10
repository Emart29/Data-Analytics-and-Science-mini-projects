# 🏙️ Airbnb Listings Analysis — New York Private Rooms  

## 📊 Project Overview  
As a **consultant for a real estate start-up**, this project analyzes **Airbnb listing data** collected from multiple sources to uncover insights about the **short-term rental market in New York**, with a focus on **private rooms**.  

The analysis combines and processes datasets from different file formats to extract useful insights such as review periods, private room counts, and pricing trends.  

---

## 🎯 Objectives  
- Determine the **earliest and most recent review dates** among all listings.  
- Count how many **Airbnb listings are private rooms**.  
- Calculate the **average listing price** (rounded to two decimal places).  
- Combine the derived insights into a single summary DataFrame called **`review_dates`**.  

---

## 📂 Dataset Description  
The project uses data from three different files located in the `/data` folder:  

| File Name | Format | Description |
|------------|---------|-------------|
| `airbnb_price.csv` | CSV | Contains listing prices and other price-related attributes |
| `airbnb_room_type.xlsx` | Excel | Describes room types for each listing |
| `airbnb_last_review.tsv` | TSV | Contains information on the most recent reviews |

---

## 🧮 Key Analysis Steps  
1. **Loaded and cleaned** data from CSV, Excel, and TSV files.  
2. **Merged datasets** using a common listing identifier.  
3. Extracted **earliest (`first_reviewed`)** and **most recent (`last_reviewed`)** review dates.  
4. Counted the number of **private room listings** (`nb_private_rooms`).  
5. Computed the **average price** (`avg_price`) of all listings, rounded to two decimal places.  
6. Combined results into a **single-row DataFrame**:

| first_reviewed | last_reviewed | nb_private_rooms | avg_price |
|-----------------|----------------|------------------|-----------|
| 2019-01-01 | 2019-07-09 | 11356 | 141.78 |

---

## 🛠 Tools & Libraries Used  
- **Python**  
- **Pandas**  
- **NumPy**  
- **Jupyter Notebook**

---

## 📁 Project Files  
| File | Description |
|------|-------------|
| `notebook.ipynb` | Main analysis notebook |
| `airbnb_price.csv` | Airbnb pricing data |
| `airbnb_room_type.xlsx` | Airbnb room type data |
| `airbnb_last_review.tsv` | Airbnb review date data |

---

## 💡 Insights for the Real Estate Company  
- **Review timelines** reveal market activity and recency of stays.  
- **Private room count** highlights opportunities for affordable accommodation investment.  
- **Average price** provides a baseline for pricing strategy and market competitiveness.  

---

## 🧾 Example Output Variables  
```python
first_reviewed = '2019-01-01'
last_reviewed = '2019-07-09'
nb_private_rooms = 11356
avg_price = 141.78
```


