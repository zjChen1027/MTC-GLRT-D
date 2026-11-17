<div align="center">

# 📡 MTC-GLRT-D

**标定数据集 · 采集配置 · 实验环境**

![Dataset](https://img.shields.io/badge/Dataset-Calibration-2563EB?style=for-the-badge)
![Radar](https://img.shields.io/badge/Radar-mmWave-7C3AED?style=for-the-badge)
![MIMO](https://img.shields.io/badge/MIMO-TDM-0891B2?style=for-the-badge)
[![Download](https://img.shields.io/badge/Download-Baidu_Netdisk-16A34A?style=for-the-badge)](https://pan.baidu.com/s/1R-9-_CCB2h_Ijt3UUY-XQA?pwd=533z)

[简体中文](README.md) · [English](README.en.md)

</div>

---

## 🔵 项目概览

本仓库用于组织 MTC-GLRT-D 算法相关的标定数据资源，提供采集配置、操作日志、实验环境与设备布置照片，以及原始数据的下载入口，便于了解采集条件并在本地开展算法实验。

| 资源 | 存放位置 | 内容 |
| :--- | :--- | :--- |
| 采集配置与日志 | GitHub | 2 个 JSON 文件、1 个 TXT 日志 |
| 实验环境与设备照片 | GitHub | 6 张 JPG 照片 |
| 原始标定数据 | 百度网盘 | 通过下方入口下载 |

## 🟢 数据集下载

> **下载入口：[百度网盘 · Calibration Dataset](https://pan.baidu.com/s/1R-9-_CCB2h_Ijt3UUY-XQA?pwd=533z)**  
> **提取码：`533z`**

原始 BIN 数据文件通过百度网盘提供。GitHub 仓库保留配置、日志和环境图，便于直接浏览；下载数据后，请保留原有文件名与目录结构，并将算法中的输入路径指向本地数据位置。

## 🟣 仓库结构

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
### 文件用途

| 文件 / 目录 | 用途 |
| :--- | :--- |
| [`Configuration File`](Calibration%20Dataset/Configuration%20File/) | 查看采集配置、设置文件与操作日志 |
| `Cascade_Capture_26.11.03.mmwave.json` | 查看各设备的射频、ADC、chirp 与 frame 配置 |
| `Cascade_Capture_26.11.03.setup.json` | 查看采集硬件、设备型号、软件版本和原始路径 |
| `Cascade_Capture_26.11.03_LogFile.txt` | 查阅采集过程中的 API 操作记录 |
| [`Environmental Equipment Diagram`](Calibration%20Dataset/Environmental%20Equipment%20Diagram/) | 查看实验环境与设备布置照片 |

## 🟠 采集配置摘要

下表摘录自仓库中的 `Cascade_Capture_26.11.03.mmwave.json` 和 `.setup.json`，描述该配置文件中的设置，**不代表网盘内全部采集批次均采用相同参数**。

| 配置项 | 配置值 |
| :--- | :--- |
| 设备型号 / 采集硬件 | AWR2243 / TDA2XX |
| mmWave Studio 版本 | 3.0.0.14 |
| 配置中的设备数 | 4（Device ID：0–3） |
| MIMO 方式 | TDM |
| 起始频率 | 77 GHz |
| 调频斜率 | 约 120.023 MHz/μs |
| ADC 采样点数 | 256 |
| ADC 采样率 | 9000 ksps（9 MS/s） |
| Idle time / ADC start time | 67 μs / 4 μs |
| Ramp end time | 33 μs |
| Chirp 索引范围 | 0–11 |
| 每帧循环数 | 64 |
| 配置帧数 / 帧周期 | 20 / 100 ms |

具体处理应以对应批次的实际配置与文件内容为准。上述参数用于说明采集设置，不构成对数据完整性、实测性能或算法结果的验证。

## 🖼️ 实验环境与设备布置

以下图片保留原文件名称，按文件名排序展示；编号仅用于浏览，不表示采集顺序或场景类别。点击图片可查看原图。

| 照片 1 | 照片 2 |
| :---: | :---: |
| [![环境与设备照片 1](Calibration%20Dataset/Environmental%20Equipment%20Diagram/06035a50d15f4775a2393283a1899121.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/06035a50d15f4775a2393283a1899121.jpg) | [![环境与设备照片 2](Calibration%20Dataset/Environmental%20Equipment%20Diagram/11df8ece23c167166d28326591db0bcf.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/11df8ece23c167166d28326591db0bcf.jpg) |

| 照片 3 | 照片 4 |
| :---: | :---: |
| [![环境与设备照片 3](Calibration%20Dataset/Environmental%20Equipment%20Diagram/19d830af0e1472c641ee7a5c3600da85.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/19d830af0e1472c641ee7a5c3600da85.jpg) | [![环境与设备照片 4](Calibration%20Dataset/Environmental%20Equipment%20Diagram/565b62ec3a75118f769142abdf380e31.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/565b62ec3a75118f769142abdf380e31.jpg) |

| 照片 5 | 照片 6 |
| :---: | :---: |
| [![环境与设备照片 5](Calibration%20Dataset/Environmental%20Equipment%20Diagram/8b4cd2c4caeeea50c7f8e0550134719b.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/8b4cd2c4caeeea50c7f8e0550134719b.jpg) | [![环境与设备照片 6](Calibration%20Dataset/Environmental%20Equipment%20Diagram/cb6cea3e4ba5ab3d72555dcfa441aa4a.jpg)](Calibration%20Dataset/Environmental%20Equipment%20Diagram/cb6cea3e4ba5ab3d72555dcfa441aa4a.jpg) |

## 🧭 使用流程与复现说明

1. **获取数据**：通过百度网盘下载原始标定数据，保留目录与文件名。
2. **核对采集条件**：阅读 JSON 配置和操作日志，结合环境图了解采集背景。
3. **设置本地路径**：在自己的处理程序中指定数据目录；如需使用配置文件，按实际环境调整其中的软件、固件和数据路径。
4. **按采集格式读取**：使用与采集格式匹配的读取程序，核对设备顺序、通道顺序、I/Q 排列和 frame/chirp 维度，再进行标定与后续处理。
5. **记录实验设置**：保存所用批次、配置文件、预处理方式和算法参数，便于复现实验。

> **路径说明**：配置文件保留原始采集内容，其中的 `E:\Ti\...` 等绝对路径属于原始计算机环境，使用前请根据本机目录调整。

当前仓库提供数据资源说明与采集材料，不包含 BIN 读取器、算法实现或完整复现实验脚本。网盘下载入口由数据提供者给出，本次文档整理未对网盘中的数据逐项下载核验。

---

<div align="center">

**📡 MTC-GLRT-D · 标定数据资源**  
[数据集下载](https://pan.baidu.com/s/1R-9-_CCB2h_Ijt3UUY-XQA?pwd=533z) · [English documentation](README.en.md)

</div>
