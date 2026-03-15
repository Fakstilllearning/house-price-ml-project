🏠 House Price Prediction - Machine Learning Project

    📌 Project Overview

        Project ini bertujuan untuk membangun model Machine Learning yang dapat memprediksi harga rumah berdasarkan berbagai fitur seperti:

            1. luas rumah
            2. jumlah kamar tidur
            3. jumlah kamar mandi
            4. jumlah lantai
            5. tahun pembangunan
            6. lokasi rumah
            7. kondisi rumah
            8. keberadaan garasi

        Model dilatih menggunakan dataset perumahan dan digunakan untuk mempelajari hubungan antara fitur-fitur rumah dengan harga.

        Project ini dibuat sebagai portfolio Data Science / Machine Learning untuk mempelajari proses Machine Learning end-to-end.

    🎯 Objectives

        Tujuan dari project ini adalah:

            1. memahami proses data analysis
            2. melakukan exploratory data analysis (EDA)
            3. melakukan data preprocessing
            4. membangun model Machine Learning
            5. membandingkan performa beberapa model
            6. melakukan evaluasi model
            7. membuat visualisasi data yang informatif

    📂 Project Structure

        house-price-ml-project
        │
        ├── data
        │   └── HousePricePredictionDataset.csv
        │
        ├── notebook
        │   └── house_price_analysis.ipynb
        │
        ├── model
        │   └── house_price_model.pkl
        │
        └── README.md

        |  Folder   |               Deskripsi                 |
        | --------- | --------------------------------------- |
        | data      | berisi dataset yang digunakan           |
        | notebook  | berisi analisis data dan training model |
        | model     | menyimpan model yang sudah dilatih      |
        | README.md | dokumentasi project                     |

    📊 Dataset

        Dataset yang digunakan berisi 2000 data rumah dengan beberapa fitur:

        |  Feature  |       Deskripsi        |
        | --------- | ---------------------- |
        | Area      | luas rumah             |
        | Bedrooms  | jumlah kamar tidur     |
        | Bathrooms | jumlah kamar mandi     |
        | Floors    | jumlah lantai          |
        | YearBuilt | tahun pembangunan      |
        | Location  | lokasi rumah           |
        | Condition | kondisi rumah          |
        | Garage    | apakah memiliki garasi |
        | Price     | harga rumah            |

        Target yang diprediksi adalah Price.

    🔎 Exploratory Data Analysis (EDA)

        Beberapa analisis yang dilakukan:

        1. Distribusi Harga Rumah

            Mengetahui distribusi harga rumah pada dataset.

        2. Hubungan Luas Rumah dan Harga

            Visualisasi scatter plot untuk melihat hubungan antara Area vs Price.

        3. Analisis Berdasarkan Jumlah Kamar

            Melihat pengaruh jumlah kamar terhadap harga rumah.

        4. Correlation Matrix

            Heatmap digunakan untuk melihat hubungan antar fitur.

    ⚙️ Data Preprocessing

        Tahapan preprocessing yang dilakukan:

            1. menghapus kolom ID
            2. melakukan encoding data kategori
            3. memisahkan fitur dan target
            4. melakukan train-test split

        Encoding dilakukan menggunakan: pd.get_dummies()

    🤖 Machine Learning Models

        Dalam project ini digunakan dua model Machine Learning:

            1️⃣ Linear Regression

                Model dasar untuk regresi yang mencoba menemukan hubungan linear antara fitur dan harga rumah. Kelebihannya yaitu sederhana dan mudah diinterpretasikan.

            2️⃣ Random Forest Regressor

                Model ensemble yang menggunakan banyak decision tree untuk meningkatkan akurasi prediksi. Kelebihannya yaitu mampu menangkap hubungan kompleks dan biasanya lebih akurat dibanding linear regression.

    📈 Model Evaluation

        Model dievaluasi menggunakan beberapa metrik:

            1. Mean Absolute Error (MAE)

                Mengukur rata-rata error prediksi.

            2. Mean Squared Error (MSE)

                Menghitung error dengan kuadrat.

            3. R² Score

                Menunjukkan seberapa baik model menjelaskan variasi data.

        Nilai:

        0 → model buruk
        1 → model sangat baik            

    📊 Visualization

        Beberapa visualisasi yang dibuat dalam project ini:

            1. distribusi harga rumah

            2. hubungan area dengan harga

            3. boxplot jumlah kamar

            4. correlation heatmap

            5. actual vs predicted price

            6. feature importance (Random Forest)

        Visualisasi dibuat menggunakan Matplotlib dan Seaborn.

    🧠 Feature Importance

        Menggunakan model Random Forest untuk melihat fitur yang paling berpengaruh terhadap harga rumah.

        Contoh fitur penting:

            1. Area
            2. Location
            3. Bedrooms
            4. Bathrooms

    💾 Model Saving

        Model yang sudah dilatih disimpan menggunakan joblib. File model disimpan di folder: model/house_price_model.pkl

        Model ini dapat digunakan kembali tanpa perlu training ulang.

    🛠️ Technologies Used

        Project ini menggunakan beberapa teknologi berikut:

        |    Tools     |         Fungsi           |
        | ------------ | ------------------------ |
        | Python       | bahasa pemrograman utama |
        | Pandas       | manipulasi data          |
        | NumPy        | operasi numerik          |
        | Matplotlib   | visualisasi data         |
        | Seaborn      | visualisasi statistik    |
        | Scikit-learn | machine learning         |

    🚀 How to Run This Project

        1. Clone repository

            git clone https://github.com/Fakstilllearning/house-price-ml-project.

        2. Install dependencies

            pip install pandas numpy matplotlib seaborn scikit-learn joblib.

        3. Jalankan notebook

            Jalankan menggunakan jupyter notebook.

        4. Buka file

            Buka file dengan nama house_price_analysis.ipynb.

    