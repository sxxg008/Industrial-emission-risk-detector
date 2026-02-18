# Industrial-emission-risk-detector
Industrial Air Audit Tool  A lightweight executable tool for automatic detection of abnormal SO2/NO2 emission events from industrial monitoring data.  No Python environment required.  Just download, double-click, and analyze.#

工业空气审计工具，一款轻量级可执行工具，可基于工业监测数据，**自动识别二氧化硫（SO₂）/二氧化氮（NO₂）排放异常事件**。无需配置Python运行环境，下载即用，双击运行即可开展分析。---本工具主要用于工业AI落地闭环能力展示


This repository is for demonstration purposes only. Sample data included.
本代码仓库仅用于演示，内含示例数据。

---------------------------------------------------------

详细说明（中英）
----------------------------------------------------------

# 工业废气审计工具

## 概述

人工核查工业环境监测数据不仅效率低下，而且结果可靠性差。

本工具可基于预定义规则对大规模监测数据进行批量自动筛查，生成污染物按小时级别联动的风险审计表。

本项目是本人工业 AI 工作流端到端能力的一个小型落地 Demo。
所有工作均由本人独立完成，包括数据获取、数据清洗、问题定义、建模、调试与封装。

### 内容

1. 下载 **data** 文件夹与 **run.exe**，放入同一目录，双击 **run.exe** 即可执行。
   程序会自动生成 **outputs** 文件夹以及 **risk_table.csv**（多污染物联动风险审计表）。

2. **examples** 文件夹包含：

   * houston_case.ipynb
   * filtering_demo.ipynb

3. **screenshots of results** 文件夹包含：

   * 休斯顿风险地图.png
   * risk_table.csv 风险排名表.png
   * 休斯顿联动异常动画截图.png

第 2–3 项主要用于展示项目发展过程，与主程序独立。

---

## 本工具可自动实现以下功能

* 检测二氧化硫（SO₂）/ 二氧化氮（NO₂）浓度异常飙升现象
* 识别多污染物复合排放异常事件
* 按核查优先级对排放站点进行排序
* 生成风险评估表及可视化分析结果

---

## 适用人群 / 机构

* 环境监管部门
* 企业合规管理团队
* 环境咨询公司

---

## 功能特点

✔ 异常排放事件自动识别

✔ 多污染物关联性分析

✔ 核查优先级风险排序

✔ 生成可直接用于报告的 CSV 输出文件

✔ 独立可执行文件（EXE）——无需安装 Python 环境

---

## 使用方法

### 1. 下载文件

* run.exe 可执行文件
* data 文件夹（原始数据表格位于 raw 子文件夹）

双击 **run.exe**，即可在 **outputs** 文件夹中生成风险筛查表。

---

### 2. 数据格式要求

替换 CSV 文件必须包含以下列名：

site_id
datetime
SO2
NO2

------------------------

# Industrial Emission Risk Audit Tool

## Overview

Manual verification of industrial environmental monitoring data is inefficient and often unreliable.

This tool automatically performs large-scale screening of monitoring datasets based on predefined rules and generates an hourly **multi-pollutant linkage risk table**.

This project serves as a small demo showcasing the **end-to-end capability of my Industrial AI workflow**, including data acquisition, cleaning, problem definition, modeling, debugging, and packaging — all completed independently.

### Contents

1. Download the **data** folder and **run.exe**, place them in the same directory, and double-click **run.exe**.
   The program will automatically generate an **outputs** folder and a file named **risk_table.csv** (multi-pollutant linkage risk audit table).

2. The **examples** folder contains:

   * houston_case.ipynb
   * filtering_demo.ipynb

3. The **screenshots of results** folder contains:

   * Houston risk map.png
   * risk_table.csv ranking table.png
   * Houston linkage anomaly animation screenshot.png

Items 2–3 mainly illustrate the project development process and are independent from the main executable program.

---

## What This Tool Does

The tool automatically enables:

* Detection of abnormal spikes in **SO₂** / **NO₂** concentrations
* Identification of multi-pollutant composite emission anomalies
* Ranking of emission sites by inspection priority
* Generation of risk tables and visual analytical outputs

---

## Target Users / Organizations

* Environmental regulatory agencies
* Corporate compliance management teams
* Environmental consulting firms

---

## Key Features

✔ Automatic abnormal emission detection

✔ Multi-pollutant correlation analysis

✔ Risk-based inspection priority ranking

✔ CSV output ready for direct reporting use

✔ Standalone executable (EXE) — no Python environment required

---

## How to Use

### 1. Download required files

* run.exe executable
* data folder (raw datasets are inside the **raw** subfolder)

Double-click **run.exe**, and the **risk screening table** will be generated automatically inside the **outputs** folder.

---

### 2. Data Format Requirement

Any replacement CSV file must include the following columns:

site_id
datetime
SO2
NO2

