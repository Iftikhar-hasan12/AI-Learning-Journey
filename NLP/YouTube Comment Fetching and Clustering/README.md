
# 🎥 YouTube Comment Fetching with Python

This project demonstrates how to **fetch comments from YouTube videos** using Python.  
The notebook provides a step-by-step guide to accessing YouTube comments through the API and processing them for further use.  

---

## 📌 Project Overview
- Connect to the **YouTube Data API**
- Retrieve video comments
- Store comments in a structured format (DataFrame)
- Perform basic text processing (cleaning)
- Perform clustering on the comments (positive or Negative or Neutral )

---

## 🚀 Technologies Used
- **Python 3**
- **pandas** → storing & handling comments in DataFrame
- **googleapiclient.discovery** → to connect with YouTube Data API
- **re (Regular Expressions)** → cleaning comment text

---

## ⚙️ Workflow
1. **API Setup**  
   - Use the YouTube Data API with an API key.  
   - Connect using `googleapiclient.discovery.build`.

2. **Fetch Comments**  
   - Extract comments, author details, and metadata from a given video ID.  

3. **Data Processing**  
   - Store results in pandas DataFrame.  
   - Clean and preprocess text (remove special characters, etc.).  

4. **Machine Learning Model Building**
    - Build K-means clustering 
    
   
