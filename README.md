# KAI-2026-passenger-forecasting-analytics

# Open Data Source Analysis & Planning Project

## Team Project
Eksplorasi sumber data terbuka (*Open Data*) yang digunakan untuk analisis dan perencanaan sistem analitik.

### Aktivitas Project
- Eksplorasi sumber data terbuka
  - Data pemerintah (`data.go.id`, `bps.go.id`, `bi.go.id`)
  - Dataset Kaggle
  - Public APIs (Calendar Worldwide API)
  - Open Research Data
- Analisis karakteristik dan kualitas data
- Membuat peta alur data untuk integrasi
- Dokumentasi requirement dan rencana penggunaan

### Output Project
- Project Blueprint  
- Project Documentation  

---

# Project Information

| Field | Information |
|------|-------------|
| **Project Name** | KAI 2026 Passenger Forecasting Analytics |
| **Created By** | Data Engineering Team 5 |
| **Date** | February 18, 2026 |
| **Version** | 1.0 |

---

# 1. Executive Summary

## 1.1 Project Overview

**Tujuan Project**  
Mengembangkan sistem analitik untuk memprediksi lonjakan penumpang kereta api jarak jauh pada masa angkutan tahun 2026.

**Scope Project**
- Data penumpang kereta api
- Data inflasi ekonomi
- Worldwide kalender (API)
- Pengembangan model Machine Learning *(Time-Series Forecasting)*

**Expected Outcomes**
- Model Machine Learning *(Facebook Prophet)* yang terlatih
- Hasil analitik prediksi jumlah penumpang kereta api tahun 2026

**Timeline**
- Maret 2026 – Mei 2026 (3 Bulan)

---

## 1.2 Stakeholders

### Project Owner
- **PT. Kereta Api Indonesia (Persero)**

### Team Members
| Role | Name |
|-----|------|
| Data Engineer | Edwin Nur Cahyo |
| Data Analyst | Dheandra Khairunnisa P |
| Project Manager | Julyo Firnanda |

### End Users
- Dinas Perhubungan  
- PT. Kereta Api Indonesia (Persero)  
- Masyarakat Umum  

---

# 2. Data Source Analysis

## 2.1 Data Pemerintah (bps.go.id)

### 2.1.1 Jumlah Penumpang Kereta Api

#### Source Details

| Field | Information |
|------|-------------|
| Dataset Name | Jumlah Penumpang Kereta Api (Ribu Orang), 2025 |
| URL | https://www.bps.go.id/id/statistics-table/2/NzIjMg==/jumlah-penumpang-kereta-api.html |
| Data Owner | Badan Pusat Statistik (BPS) |
| Update Frequency | Bulanan |

#### Data Analysis

| Metric | Description |
|------|-------------|
| Format Data | CSV |
| Volume Data | 940 B |
| Time Coverage | Januari 2007 – Februari 2026 |
| Completeness | 99% |
| Accuracy | High (Verified by Dishub & PT KAI) |
| Consistency | Good |
| Timeliness | Last Updated 2 Februari 2026 |

---

### 2.1.2 Inflasi Indeks Harga Konsumen (IHK)

#### Source Details

| Field | Information |
|------|-------------|
| Dataset Name | Inflasi Indeks Harga Konsumen (IHK) |
| URL | https://www.bi.go.id/id/statistik/indikator/data-inflasi.aspx |
| Data Owner | Bank Indonesia |
| Update Frequency | Bulanan |

#### Data Analysis

| Metric | Description |
|------|-------------|
| Format Data | HTML Table / XLSX |
| Data Fields | Inflasi IHK (YoY), Target Inflasi, BI Rate, MtM, YtD |
| Time Coverage | Hingga Februari 2026 |
| Completeness | 100% |
| Accuracy | Tinggi |
| Consistency | Sangat Baik |
| Timeliness | Update setiap rilis data bulanan |

---

### 2.1.3 Inflasi Umum

#### Source Details

| Field | Information |
|------|-------------|
| Dataset Name | Inflasi (Umum) 2006 – 2026 |
| URL | https://www.bps.go.id/id/statistics-table/2/MSMy/inflasi--umum-.html |
| Data Owner | Badan Pusat Statistik |
| Update Frequency | Bulanan |

#### Data Analysis

| Metric | Description |
|------|-------------|
| Format Data | CSV / XLSX |
| Data Fields | Bulan, Tahun, Tingkat Inflasi |
| Time Coverage | Januari 2006 – Februari 2026 |
| Completeness | 100% |
| Accuracy | Tinggi |
| Consistency | Sangat Konsisten |
| Timeliness | Update setiap awal bulan |

---

## 2.2 Dataset Kaggle

#### Source Details

| Field | Information |
|------|-------------|
| Dataset Name | Inflation Rate in Asia |
| URL | https://www.kaggle.com/datasets/utkarshx27/inflation-rate-in-asia |
| Creator | Utkarsh Singh |
| Last Update | 3 Years Ago |

#### Data Analysis

| Metric | Description |
|------|-------------|
| Format | CSV |
| Size | 16.46 KB |
| Data Fields | RegionalMember, Year, Inflation, Unit Of Measurement, Subregion, Country Code |
| Missing Values | 4% |
| Data Types | Numeric & Categorical |
| Consistency | High |
| Documentation | Excellent (Includes Data Dictionary) |

---

## 2.3 Public APIs

#### Source Details

| Field | Information |
|------|-------------|
| API Name | Global Holiday Calendar API |
| Endpoint | https://calendarific.com/api/v2/holidays |
| Provider | Calendarific |
| Authentication | API Key |

#### API Analysis

| Metric | Description |
|------|-------------|
| Response Format | JSON |
| Rate Limit | 1000 Request / Day |
| Reliability | 99.9% Uptime |
| Documentation | Comprehensive |
| Cost | Free Tier (1000 request/day) |

---

## 2.4 Open Research Data

#### Source Details

| Field | Information |
|------|-------------|
| Dataset Name | Applied of Feed-Forward Neural Network and Facebook Prophet Model for Train Passengers Forecasting |
| Repository | IOP Publishing |
| Research Institution | Universitas Padjadjaran |
| Publication Year | 2021 |

#### Data Analysis

| Metric | Description |
|------|-------------|
| Format | Journal PDF |
| Data Volume | 928 KB |
| Access | Open Access |
| Citation | https://iopscience.iop.org/article/10.1088/1742-6596/1776/1/012057 |
