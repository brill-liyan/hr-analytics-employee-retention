# 📊 Data Analysis: Employee Retention Strategy

Analisis data untuk mengidentifikasi faktor-faktor yang memengaruhi **employee attrition** serta merumuskan strategi retensi karyawan berbasis data pada PT Vinix Seven Aurum.

> **Project Type:** Data Analysis & HR Analytics
> **Methodology:** CRISP-DM
> **Tools:** Python, Pandas, Matplotlib, Seaborn, Google Colab, Looker Studio
> **Dataset:** IBM HR Analytics Employee Attrition & Performance

## 📌 Project Overview

Employee attrition atau keluarnya karyawan merupakan salah satu permasalahan strategis yang dapat berdampak pada biaya rekrutmen, pelatihan ulang, produktivitas, serta stabilitas organisasi.

Proyek ini dilakukan untuk menganalisis pola employee attrition menggunakan pendekatan **data-driven**. Analisis berfokus pada identifikasi faktor-faktor yang berkaitan dengan keputusan karyawan untuk meninggalkan perusahaan serta karakteristik kelompok karyawan yang memiliki risiko attrition lebih tinggi.

Hasil analisis kemudian diterjemahkan ke dalam **interactive dashboard** untuk membantu menyajikan insight secara lebih mudah dipahami dan mendukung pengambilan keputusan strategis.

## 🎯 Business Questions

Analisis ini dilakukan untuk menjawab beberapa pertanyaan bisnis:

1. Seberapa besar tingkat attrition karyawan?
2. Faktor apa saja yang memiliki keterkaitan dengan tingginya attrition?
3. Kelompok karyawan seperti apa yang paling rentan melakukan attrition?
4. Bagaimana hasil analisis dapat digunakan untuk merumuskan strategi retensi yang lebih tepat sasaran?

## 📂 Dataset

Dataset yang digunakan adalah **IBM HR Analytics Employee Attrition & Performance** yang terdiri dari:

* **1.470 baris data karyawan**
* **35 variabel awal**
* Target variable: `Attrition`

Beberapa variabel yang dianalisis meliputi:

### 💼 Job & Compensation

* `JobRole`
* `JobLevel`
* `MonthlyIncome`
* `OverTime`

### 😊 Employee Satisfaction

* `JobSatisfaction`
* `EnvironmentSatisfaction`
* `WorkLifeBalance`
* `RelationshipSatisfaction`

### 🏢 Organizational Factors

* `Department`
* `YearsAtCompany`
* `YearsInCurrentRole`
* `YearsSinceLastPromotion`

### 👤 Demographic Factors

* `Age`
* `Gender`
* `MaritalStatus`
* `DistanceFromHome`

> Dataset yang digunakan merupakan dataset analisis HR yang tersedia untuk keperluan analisis dan pembelajaran. Pastikan file dataset yang diunggah ke repository tidak mengandung data perusahaan atau data pribadi yang bersifat sensitif.

## 🔄 Methodology

Proyek ini menggunakan framework **CRISP-DM (Cross-Industry Standard Process for Data Mining)**.

### 1. Business Understanding

Menentukan permasalahan bisnis, tujuan analisis, pertanyaan bisnis, dan metrik utama yang akan dianalisis.

### 2. Data Understanding

Melakukan eksplorasi terhadap dataset, termasuk:

* Struktur data
* Tipe variabel
* Distribusi data
* Kualitas data
* Missing values

### 3. Data Preparation

Tahap data preparation meliputi:

* Pemeriksaan kualitas data
* Penghapusan kolom yang tidak relevan
* Transformasi variabel target
* Feature engineering
* Binning variabel numerik

Beberapa fitur turunan yang dibuat:

* `Attrition_Binary`
* `Age_Group`
* `Income_Level`
* `Working_Years_Group`
* `Distance_Group`

Kolom yang tidak relevan atau bersifat konstan dihapus agar analisis lebih fokus.

### 4. Exploratory Data Analysis (EDA)

Analisis eksploratif dilakukan untuk menemukan pola dan hubungan antara berbagai faktor dengan employee attrition.

Analisis meliputi:

* Korelasi antar fitur numerik
* Attrition berdasarkan fitur kategorikal
* Analisis demografi
* Analisis faktor pekerjaan dan kompensasi
* Analisis kepuasan kerja dan work-life balance
* Analisis berdasarkan pertanyaan bisnis

### 5. Evaluation

Insight yang dihasilkan dievaluasi berdasarkan:

* Konsistensi data
* Kualitas proses data preparation
* Konsistensi antarvisualisasi
* Relevansi terhadap permasalahan bisnis
* Kemudahan interpretasi bagi stakeholder non-teknis

### 6. Deployment

Hasil analisis disajikan dalam bentuk:

* Interactive dashboard
* Laporan analisis
* Presentasi proyek

## 📊 Key Findings

### 1. Attrition Rate Mencapai 16,2%

Tingkat attrition sebesar **16,2%** menunjukkan adanya tantangan retensi yang perlu mendapatkan perhatian strategis.

### 2. Karyawan dengan Pendapatan Rendah Lebih Rentan Mengalami Attrition

Kelompok karyawan dengan tingkat pendapatan rendah menunjukkan risiko attrition yang lebih tinggi.

Pada analisis, karyawan dengan pendapatan rendah berkontribusi terhadap jumlah attrition yang besar. Hal ini menunjukkan pentingnya evaluasi terhadap struktur kompensasi, terutama pada posisi dan job level yang lebih rendah.

### 3. Job Level Rendah Memiliki Risiko Attrition Lebih Tinggi

Karyawan pada **Job Level 1** memiliki jumlah attrition tertinggi dibandingkan level lainnya.

Hal ini dapat mengindikasikan adanya tantangan terkait:

* Pengembangan karier
* Kompensasi
* Kepuasan kerja
* Kesempatan peningkatan skill

### 4. Overtime Berkaitan dengan Tingginya Attrition

Karyawan yang melakukan overtime menunjukkan tingkat attrition yang lebih tinggi dibandingkan karyawan yang tidak melakukan overtime.

Temuan ini menunjukkan pentingnya pengelolaan:

* Beban kerja
* Distribusi tugas
* Batas lembur
* Keseimbangan antara pekerjaan dan kehidupan pribadi

### 5. Work-Life Balance dan Job Satisfaction Berperan dalam Retensi

Karyawan dengan tingkat **Work-Life Balance** dan **Job Satisfaction** yang rendah cenderung memiliki risiko attrition yang lebih tinggi.

Hal ini menunjukkan bahwa strategi retensi tidak hanya perlu berfokus pada kompensasi, tetapi juga pada pengalaman kerja dan kesejahteraan karyawan.

### 6. Segmen Job Level Rendah dan Low Income Menjadi Area Risiko Utama

Hasil analisis menunjukkan bahwa kombinasi antara **job level rendah** dan **income level rendah** merupakan salah satu segmen yang memiliki risiko attrition paling tinggi.

Segmen ini dapat menjadi prioritas utama dalam perancangan strategi retensi.

## 💡 Strategic Recommendations

Berdasarkan hasil analisis, beberapa rekomendasi yang dapat dipertimbangkan:

### 💰 1. Evaluasi Struktur Kompensasi
Melakukan salary benchmarking untuk posisi dan kelompok karyawan yang memiliki risiko attrition tinggi.
### ⏱️ 2. Mengelola Beban Kerja dan Overtime
Melakukan evaluasi terhadap distribusi beban kerja serta menerapkan kebijakan lembur yang lebih terukur.
### 📈 3. Membangun Jalur Karier yang Lebih Jelas
Menyediakan career roadmap, mentoring, dan program upskilling khususnya bagi karyawan pada job level awal.
### 🧘 4. Meningkatkan Employee Well-being
Meningkatkan dukungan terhadap work-life balance, employee satisfaction, serta kesejahteraan karyawan.

## 📈 Dashboard

Dashboard interaktif dibuat menggunakan **Looker Studio** untuk menyajikan:
* Attrition Rate
* Attrition berdasarkan Monthly Income
* Attrition berdasarkan Job Level
* Attrition berdasarkan Job Role
* Analisis OverTime
* Analisis Work-Life Balance
* Heatmap risiko berdasarkan Job Level dan Income Level
* Segmentasi karyawan berdasarkan berbagai karakteristik

🔗 **View Interactive Dashboard:**
[https://datastudio.google.com/reporting/5656ba0f-c145-41f0-81d4-fe866ac471f2]


## 🛠️ Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Google Colab**
* **Looker Studio**
* **GitHub**

## 📁 Repository Structure

```text
employee-retention-analysis/
│
├── data/
│   └── HR_Dataset_Clean.csv
│
├── notebooks/
│   └── employee_retention_analysis.ipynb
│
├── dashboard/
│   ├── dashboard_screenshot.png
│   └── dashboard_preview.pdf
│
├── report/
│   └── project_report.pdf
│
├── README.md
└── requirements.txt
```


## 👩‍💻 My Contribution

Dalam proyek kelompok ini, saya berkontribusi dalam proses:

* Data preparation dan data cleaning
* Feature engineering
* Exploratory Data Analysis
* Analisis faktor-faktor yang berkaitan dengan employee attrition
* Pengembangan insight untuk dashboard
* Penyusunan rekomendasi strategis berbasis hasil analisis
* Dokumentasi dan presentasi hasil proyek


## 📚 Project Deliverables

* 📓 **Google Colab / Jupyter Notebook** – Data preparation & EDA
* 📊 **Looker Studio Dashboard** – Interactive data visualization
* 📄 **Final Project Report** – Dokumentasi analisis
* 🎤 **Final Presentation** – Presentasi hasil proyek

## 👥 Team

This project was completed as a group project during the **VINIX7 Independent Study Program – Junior Data Scientist Division**.

**Team 19:**
* Adellia Nirma Azzahra
* Alfirda Ananda Firdauz
* Andrian Simanjuntak
* Aurora Euniqe Azzahra Eriawan
* Brilliyanda Annisaatulrohmah
* Finarti

## 📌 Note

This project was developed as part of a data analysis project during the VINIX7 Independent Study Program. The analysis focuses on identifying patterns and potential factors associated with employee attrition using historical HR data.

The findings should be interpreted as analytical insights and should be complemented with additional organizational context before being used for actual HR policy decisions.
