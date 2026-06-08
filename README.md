# Analisis-Tren-Ekonomi-Digital-ASEAN-Menggunakan-Data-Historis-2019-2023
Project ini untuk memenuhi Ujian Akhir Semester Mata Kuliah Data Warehouse, Semester Genap 2025/2026, Kelas 2024D, Universitas Negeri Surabaya. Project ini membangun pipeline Data Warehouse untuk menganalisis tren perdagangan jasa digital di 10 negara ASEAN periode 2019–2023 menggunakan pendekatan Ralph Kimball dengan star schema, PostgreSQL Supabase, dan Atoti.

# Anggota Kelompok:
1. Nia Ayu Agustin (24031554081)
2. Aulia Aziza (24031554102)
3. Audy Alycia (24031554179)

# Dataset
UNCTAD Digital Economy — World Indicators of Digital Economy and Finance (WIDEF)
https://data360.worldbank.org/en/dataset/UNCTAD_DE

# Metode
1. Extract: Full load dataset UNCTAD_DE_WIDEF.csv, filter 10 negara ASEAN dan indikator ekspor-impor jasa digital
2. Transform: Melt wide ke long/tidy, cleaning, pembentukan star schema (3 dimensi, 1 fact table)
3. Load: PostgreSQL Supabase dengan B-tree Index dan Materialized View untuk optimasi OLAP
4. OLAP: Atoti cube dengan hierarchy negara, waktu, dan tipe perdagangan

# Hasil
Singapura mendominasi ekspor jasa digital ASEAN dengan total 781.109 juta USD selama 2019–2023, jauh melampaui negara lainnya. Kawasan ASEAN secara keseluruhan mengalami defisit perdagangan jasa digital di seluruh periode, dengan nilai impor yang konsisten lebih tinggi dari ekspor. Hanya Singapura dan Filipina yang mencatat surplus perdagangan jasa digital.
