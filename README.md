# AI-Powered Ransomware Detection via Behavioral Forensics

This project explores deep learning architectures for ransomware detection using behavioral telemetry (RanSMAP dataset). We benchmark Autoencoders, CNNs, LSTMs, and propose a novel Dual-Channel CNN–BiLSTM model.

## 📁 Project Structure

- `Notebooks/` — All model notebooks and experiments, from baseline to hybrid architectures, contains also the preprocessing notebook that produced the parquet we're using throughout the project.
- `Datasets/` — RanSMAP dataset as a preprocessed assembled parquet file.
- `Utils/` — Scripts for assembling teh dataset , as it comes devided to many .csv files.
- `report.pdf` — Final written report of the project.

## 🚀 Main Result

Our dual-branch CNN–BiLSTM model achieved:
- **F1-score**: 92.24%
- **Recall**: 91.02%
- under a **family-aware split** (unseen ransomware families), significantly outperforming baseline models.

## 📊 Dataset

We use the [RanSMAP dataset](https://github.com/manabu-hirano/RanSMAP), which contains fine-grained storage and memory access patterns (LBA, GPA, Entropy, Read/Write/Execution counts).

## 🔧 Setup

