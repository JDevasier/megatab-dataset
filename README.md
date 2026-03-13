# MegaTab: A Dataset of Massive Tables for Automatic Fact-Checking

**To appear in LREC 2026**

[![arXiv](https://img.shields.io/badge/arXiv-2601.17232-b31b1b.svg)](https://arxiv.org/abs/2601.17232)
[![HuggingFace](https://img.shields.io/badge/%F0%9F%A4%97%20HuggingFace-Dataset-yellow)](https://huggingface.co/datasets/jdevasier/MegaTab)
[![Google Drive](https://img.shields.io/badge/Google%20Drive-OECD%20Database-4285F4?logo=googledrive&logoColor=white)](https://drive.google.com/file/d/12lMqK6a5sVAfBGguBeZBchfg-gjB9Bqi/view?usp=sharing)
[![Conference](https://img.shields.io/badge/LREC-2026-blue)](https://lrec2026.info/)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

📄 **Paper:** [Frame-Guided Synthetic Claim Generation for Automatic Fact-Checking Using High-Volume Tabular Data](https://arxiv.org/abs/2601.17232)

**Authors:** Jacob Devasier, Akshith Putta, Qing Wang, Alankrit Moses, Chengkai Li

## Abstract
Automated fact-checking benchmarks have largely ignored the challenge of verifying claims against real-world, high-volume structured data, instead focusing on small, curated tables. We introduce a new large-scale, multilingual dataset to address this critical gap. It contains 78,503 synthetic claims grounded in 434 complex OECD tables, which average over 500K rows each. We propose a novel, frame-guided methodology where algorithms programmatically select significant data points based on six semantic frames to generate realistic claims in English, Chinese, Spanish, and Hindi. Crucially, we demonstrate through knowledge-probing experiments that LLMs have not memorized these facts, forcing systems to perform genuine retrieval and reasoning rather than relying on parameterized knowledge. We provide a baseline SQL-generation system and show that our benchmark is highly challenging. Our analysis identifies evidence retrieval as the primary bottleneck, with models struggling to find the correct data in massive tables. This dataset provides a critical new resource for advancing research on this unsolved, real-world problem.

## Claims Dataset
This repository contains the test set and a small sample of the training set. 

The full train and test datasets can be downloaded from [Huggingface](https://huggingface.co/datasets/jdevasier/MegaTab): `jdevasier/MegaTab`. 

## OECD Database
We have provided two scripts to help create the OECD database. `download_datasets.py` can be used to download all of the OECD statistics data files. `csv_to_db.py` can then be used to convert all of the CSV files to a database. 

The OECD database can be downloaded from [google drive](https://drive.google.com/file/d/12lMqK6a5sVAfBGguBeZBchfg-gjB9Bqi/view?usp=sharing).
