# MTC-GLRT-D

本仓库提供用于 MTC-GLRT-D 算法的标定数据集相关采集配置与实验环境图。原始数据通过百度网盘下载。

## 数据集下载

- **百度网盘链接**：[下载 Calibration Dataset](https://pan.baidu.com/s/1R-9-_CCB2h_Ijt3UUY-XQA?pwd=533z)
- **提取码**：`533z`

## 仓库目录

```text
MTC-GLRT-D/
├── README.md
└── Calibration Dataset/
    ├── Configuration File/
    │   ├── Cascade_Capture_26.11.03.mmwave.json
    │   ├── Cascade_Capture_26.11.03.setup.json
    │   └── Cascade_Capture_26.11.03_LogFile.txt
    └── Environmental Equipment Diagram/
        └── *.jpg
```

- **Configuration File**：包含 mmWave Studio 配置文件、采集设置文件及操作日志。
- **Environmental Equipment Diagram**：包含实验环境与设备布置照片，共 6 张。

## 使用说明

1. 通过上述百度网盘链接下载标定数据集。
2. 结合配置文件了解采集设置，结合环境图查看实验场景与设备布置。
3. 在本地算法程序中指定下载数据的实际路径。

配置文件保留采集时的原始内容，其中的本地绝对路径对应原始采集环境；在其他计算机上使用时，请按实际安装与数据存储位置调整路径。

本仓库仅托管上述配置、日志和环境图；原始 BIN 数据文件通过百度网盘提供。
