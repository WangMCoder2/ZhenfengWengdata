# Synthetic IoMT Security Dataset (CSV-only)

A complete, **paper-grade synthetic dataset** for IoMT (Internet of Medical Things) cybersecurity research, designed for **reproducible experiments**, **open-source algorithm benchmarking**, and **end-to-end pipeline validation**.

This dataset strictly follows the experimental requirements described in the manuscript, covering **all required data categories without omission**.

---

## 📌 Key Features

- ✅ **CSV-only format** (easy integration with ML/DL pipelines)
- ✅ Covers **IoMT network traffic, DICOM communication, ECG signals, drug traceability**
- ✅ Includes **attack labels, severity levels, timestamps**
- ✅ Large-scale (**million-level network flows**)
- ✅ Ready for **IDS / Federated Learning / Reinforcement Learning / Anomaly Detection**
- ✅ Train / Validation / Test splits included

> ⚠️ **Note**  
> This dataset is **synthetic** and intended for method validation, algorithm development, and reproducibility.  
> If reviewers require *real public datasets*, use this dataset **together with** referenced GitHub open datasets.

---

## 📂 Directory Structure

By default, all files are generated under:


Structure:

```text
dataset/
├── README.md
├── raw/
│   ├── network/
│   │   ├── device_inventory.csv
│   │   └── flows/
│   │       ├── normal.csv
│   │       └── attack.csv
│   ├── dicom/
│   │   ├── pcap/
│   │   │   ├── dicom_sessions.csv
│   │   │   └── dicom_packets.csv
│   │   └── images/
│   │       └── dicom_files_metadata.csv
│   ├── ecg/
│   │   └── segments/
│   │       └── ecg_segments.csv
│   └── traceability/
│       ├── terminals.csv
│       ├── product_batches.csv
│       └── transactions.csv
├── labels/
│   ├── network_labels.csv
│   ├── dicom_attack_labels.csv
│   ├── ecg_injection_labels.csv
│   └── traceability_attack_labels.csv
└── splits/
    ├── train.txt
    ├── val.txt
    └── test.txt
If you use this dataset in academic work, please cite your corresponding paper/project and clearly indicate that the dataset is synthetic.
This dataset is released for research and educational purposes only.
Redistribution is permitted provided that the synthetic nature of the data is clearly stated.
