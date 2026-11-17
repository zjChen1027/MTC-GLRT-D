<div align="center">

# 📡 MTC-GLRT-D

**Calibration Dataset · Acquisition Configuration · Experimental Setup**

![Dataset](https://img.shields.io/badge/Dataset-Calibration-2563EB?style=for-the-badge)
![Radar](https://img.shields.io/badge/Radar-mmWave-7C3AED?style=for-the-badge)
![MIMO](https://img.shields.io/badge/MIMO-TDM-0891B2?style=for-the-badge)
[![Download](https://img.shields.io/badge/Download-Baidu_Netdisk-16A34A?style=for-the-badge)](https://pan.baidu.com/s/1R-9-_CCB2h_Ijt3UUY-XQA?pwd=533z)

[简体中文](README.md) · [English](README.en.md)

</div>

---

## 🔵 Overview

This repository organizes calibration resources for the MTC-GLRT-D algorithm. It provides acquisition configurations, operation logs, photographs of the experimental environment and equipment, and a download link to the raw data for local experiments.

| Resource | Location | Contents |
| :--- | :--- | :--- |
| Acquisition configurations and log | GitHub | 2 JSON files and 1 TXT log |
| Environment and equipment photographs | GitHub | 6 JPG photographs |
| Raw calibration data | Baidu Netdisk | Available through the link below |

## 🟢 Dataset Download

> **Download: [Baidu Netdisk · Calibration Dataset](https://pan.baidu.com/s/1R-9-_CCB2h_Ijt3UUY-XQA?pwd=533z)**  
> **Access code: `533z`**

Raw BIN files are distributed through Baidu Netdisk. The GitHub repository hosts configurations, the operation log, and photographs for browsing. After downloading, preserve the original filenames and directory structure, and point your algorithm's input paths to the local data location.

## 🟣 Repository Structure

```text
MTC-GLRT-D/
├── README.md                         # 中文说明
├── README.en.md                      # English documentation
└── Calibration Dataset/
    ├── Configuration File/
    │   ├── Cascade_Capture_26.11.03.mmwave.json
    │   ├── Cascade_Capture_26.11.03.setup.json
    │   └── Cascade_Capture_26.11.03_LogFile.txt
    └── Environmental Equipment Diagram/
        └── *.jpg                     # 6 photographs
```
### File Guide

| File / Directory | Purpose |
| :--- | :--- |
| [`Configuration File`](Calibration%20Dataset/Configuration%20File/) | Acquisition configurations, setup file, and operation log |
| `Cascade_Capture_26.11.03.mmwave.json` | Per-device RF, ADC, chirp, and frame configurations |
| `Cascade_Capture_26.11.03.setup.json` | Capture hardware, device model, software version, and original paths |
| `Cascade_Capture_26.11.03_LogFile.txt` | API operation records from the acquisition process |
| [`Environmental Equipment Diagram`](Calibration%20Dataset/Environmental%20Equipment%20Diagram/) | Photographs of the experimental environment and equipment arrangement |

## 🟠 Acquisition Configuration Summary

The values below are taken from `Cascade_Capture_26.11.03.mmwave.json` and `.setup.json`. They describe the settings in these files; **they do not imply that all acquisition batches in the download use the same parameters**.

| Parameter | Configured value |
| :--- | :--- |
| Device / Capture hardware | AWR2243 / TDA2XX |
| mmWave Studio version | 3.0.0.14 |
| Number of configured devices | 4 (Device IDs: 0–3) |
| MIMO scheme | TDM |
| Start frequency | 77 GHz |
| Frequency slope | Approximately 120.023 MHz/μs |
| ADC samples | 256 |
| ADC sampling rate | 9000 ksps (9 MS/s) |
| Idle time / ADC start time | 67 μs / 4 μs |
| Ramp end time | 33 μs |
| Chirp index range | 0–11 |
| Loops per frame | 64 |
| Configured frames / Frame period | 20 / 100 ms |

Use the actual configuration and files for the batch being processed. These values document acquisition settings; they do not verify data completeness, measured performance, or algorithmic results.

## 🖼️ Experimental Environment and Equipment

The images retain their original filenames and are displayed in filename order. Image numbers are for navigation only and do not indicate acquisition order or scene categories. Click an image to view the original.

| Photo 1 | Photo 2 |
| :---: | :---: |
| [![Environment and equipment photo 1](Calibration%20Dataset/Environmental%20Equipment%20Diagram/06035a50d15f4775a2393283a1899121.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/06035a50d15f4775a2393283a1899121.jpg) | [![Environment and equipment photo 2](Calibration%20Dataset/Environmental%20Equipment%20Diagram/11df8ece23c167166d28326591db0bcf.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/11df8ece23c167166d28326591db0bcf.jpg) |

| Photo 3 | Photo 4 |
| :---: | :---: |
| [![Environment and equipment photo 3](Calibration%20Dataset/Environmental%20Equipment%20Diagram/19d830af0e1472c641ee7a5c3600da85.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/19d830af0e1472c641ee7a5c3600da85.jpg) | [![Environment and equipment photo 4](Calibration%20Dataset/Environmental%20Equipment%20Diagram/565b62ec3a75118f769142abdf380e31.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/565b62ec3a75118f769142abdf380e31.jpg) |

| Photo 5 | Photo 6 |
| :---: | :---: |
| [![Environment and equipment photo 5](Calibration%20Dataset/Environmental%20Equipment%20Diagram/8b4cd2c4caeeea50c7f8e0550134719b.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/8b4cd2c4caeeea50c7f8e0550134719b.jpg) | [![Environment and equipment photo 6](Calibration%20Dataset/Environmental%20Equipment%20Diagram/cb6cea3e4ba5ab3d72555dcfa441aa4a.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/cb6cea3e4ba5ab3d72555dcfa441aa4a.jpg) |

## 🧭 Usage and Reproducibility

1. **Download the data** from Baidu Netdisk and preserve the original directory structure and filenames.
2. **Review the acquisition conditions** using the JSON configurations, operation log, and environment photographs.
3. **Set local paths** in your processing program. If you use the configuration files, adapt software, firmware, and data paths to your installation.
4. **Read the acquisition format correctly** with a compatible reader. Check device order, channel order, I/Q layout, and frame/chirp dimensions before calibration and subsequent processing.
5. **Record experimental settings**, including the acquisition batch, configuration files, preprocessing steps, and algorithm parameters.

> **Path note:** Configuration files retain their original acquisition contents. Absolute paths such as `E:\Ti\...` refer to the original computer and must be adapted to your local environment before use.

This repository provides resource documentation and acquisition materials. It does not include a BIN reader, algorithm implementation, or complete experiment reproduction scripts. The download link was supplied by the data provider; the files in Baidu Netdisk have not been individually downloaded and verified during this documentation update.

---

<div align="center">

**📡 MTC-GLRT-D · Calibration Data Resources**  
[Download dataset](https://pan.baidu.com/s/1R-9-_CCB2h_Ijt3UUY-XQA?pwd=533z) · [中文说明](README.md)

</div>
