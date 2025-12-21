# Customer-Segmentation-using-K-Means-Clustering
This repository contains an Unsupervised Machine Learning project focused on segmenting online shop customers into distinct groups based on their behavioral data.
Here is the **README file** for the Customer Segmentation (Clustering) project. 

## Author
* Nukri Munjishvili

## Project Overview
The objective of this project is to analyze customer data and identify patterns that allow for the categorization of users into clusters. This segmentation helps in understanding different customer profiles, which is essential for targeted marketing and personalized services.

## Technical Details

### Libraries Used
The project is implemented in Python using the following libraries:
* **Pandas & NumPy:** For data manipulation and numerical operations.
* **Scikit-Learn:** For data preprocessing (StandardScaler), clustering (KMeans), dimensionality reduction (PCA), and metric evaluation (Silhouette Score).
* **Matplotlib & Seaborn:** For 2D and 3D data visualization.
* **OpenPyxl:** For reading Excel files.

### Methodology
1.  **Data Preprocessing:**
    * The data was loaded from an Excel file (`.xlsx`) to ensure correct encoding of character sets.
    * **Standardization:** The `StandardScaler` was applied to normalize the feature values, ensuring that all variables contribute equally to the distance calculations.
2.  **Optimal Cluster Selection:**
    * The **Elbow Method** was utilized to determine the optimal number of clusters ($k$). The Within-Cluster Sum of Squares (WCSS) was plotted against the number of clusters.
3.  **Clustering Algorithm:**
    * **K-Means Clustering** was applied with $k=3$ (based on the Elbow Method analysis).
4.  **Visualization:**
    * **PCA (Principal Component Analysis):** Dimensionality reduction was performed to visualize the high-dimensional data in a 3D space.

## Results
The analysis resulted in the formation of 3 distinct customer clusters.
* **Evaluation:** The quality of the clustering was assessed using the **Silhouette Score**.
* **Interpretation:** A heatmap was generated to analyze the mean values of features within each cluster, providing insights into the characteristics of each customer segment.

## How to Run
1.  **File Requirement:** Ensure the data file is named `clustering_მონაცემები.xlsx`.
    * *Note:* Do not use a CSV file converted manually, as it may cause encoding errors. Use the original Excel workbook.
2.  Open the Jupyter Notebook (`ProjectCode.ipynb`).
3.  Run the cells sequentially to perform the analysis and generate the visualizations.

---

# Customer Segmentation (Georgian Version)

# მომხმარებელთა სეგმენტაცია (კლასტერინგი)

ეს რეპოზიტორია მოიცავს არაზედამხედველობითი სწავლების (Unsupervised Learning) პროექტს, რომლის მიზანია ონლაინ მაღაზიის მომხმარებლების დაჯგუფება მათი ქცევითი მახასიათებლების მიხედვით.

## ავტორი
* ნუკრი მუნჯიშვილი

## პროექტის მიმოხილვა
პროექტის მიზანია მონაცემთა ანალიზის საფუძველზე მომხმარებელთა მსგავსი ჯგუფების (კლასტერების) იდენტიფიცირება. აღნიშნული სეგმენტაცია მნიშვნელოვანია მომხმარებლის ქცევის შესასწავლად და მარკეტინგული სტრატეგიების დასაგეგმად.

## ტექნიკური დეტალები

### გამოყენებული ბიბლიოთეკები
პროექტი შესრულებულია Python-ში შემდეგი ბიბლიოთეკების გამოყენებით:
* **Pandas & NumPy:** მონაცემთა დამუშავება.
* **Scikit-Learn:** მონაცემთა სკალირება (StandardScaler), კლასტერინგი (KMeans), PCA და მეტრიკები (Silhouette Score).
* **Matplotlib & Seaborn:** მონაცემთა ვიზუალიზაცია.
* **OpenPyxl:** Excel-ის ფაილების წასაკითხად.

### მეთოდოლოგია
1.  **მონაცემთა პრეპროცესინგი:**
    * მონაცემები ჩაიტვირთა Excel-ის (`.xlsx`) ფაილიდან კოდირების პრობლემების თავიდან ასაცილებლად.
    * **სტანდარტიზაცია:** გამოყენებულ იქნა `StandardScaler`, რათა ყველა ცვლადი მოყვანილიყო ერთ მასშტაბში.
2.  **კლასტერების რაოდენობის შერჩევა:**
    * გამოყენებულ იქნა **Elbow Method** (იდაყვის მეთოდი) ოპტიმალური $k$ მნიშვნელობის დასადგენად.
3.  **ალგორითმი:**
    * მონაცემებზე გაეშვა **K-Means** ალგორითმი 3 კლასტერით ($k=3$).
4.  **ვიზუალიზაცია:**
    * **PCA:** განზომილების შემცირების მეთოდით მონაცემები ვიზუალიზდა 3D სივრცეში.

## შედეგები
ანალიზის შედეგად გამოიყო მომხმარებელთა 3 განსხვავებული ჯგუფი.
* **შეფასება:** კლასტერინგის ხარისხი შეფასდა **Silhouette Score**-ის მეშვეობით.
* **ინტერპრეტაცია:** შეიქმნა Heatmap, რომელმაც აჩვენა თითოეული კლასტერის საშუალო მაჩვენებლები და მათი მახასიათებლები.

## გაშვების ინსტრუქცია
1.  **ფაილის მოთხოვნა:** დარწმუნდით, რომ მონაცემთა ფაილის სახელია `clustering_მონაცემები.xlsx`.
    * *შენიშვნა:* გამოიყენეთ Excel-ის ორიგინალი ფაილი და არა CSV, რათა თავიდან აიცილოთ "Bad offset" შეცდომები.
2.  გახსენით Jupyter Notebook (`ProjectCode.ipynb`).
3.  გაუშვით სელები თანმიმდევრობით.
