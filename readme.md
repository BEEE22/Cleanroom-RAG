# Cleanroom Design Assistant (Multimodal RAG System)

🌟 **A Next-Generation Solution for Medical Cleanroom Design Support**  
*Empowering Healthcare Facilities and Pharmaceutical Cleanroom Engineering*

---

## 📖 Overview
This project implements a multimodal Retrieval-Augmented Generation (RAG) assistant specialized in medical cleanroom design, offering professional Q&A services and technical support for healthcare facilities and pharmaceutical production environments. The system integrates domain-specific knowledge databases with advanced AI capabilities to deliver contextualized solutions.

### Key Features
- 🏥 **Hospital Cleanroom Expertise**: Specialized in ORs, isolation wards, and sterile processing departments  
- 🧪 **Pharmaceutical Facility Support**: GMP-compliant solutions for production areas and laboratories  
- 💡 **Multimodal Intelligence**: Combines structured data, technical documents, and AI reasoning  
- 🔍 **Context-Aware Responses**: Sophisticated retrieval mechanisms for accurate technical guidance  

### ⚠️ Note
This is an early-stage prototype developed under tight time constraints.

You may encounter bugs or incomplete features.

### 🚧 Future Plans
Continuous improvements and bug fixes

Deployment as a full-featured website

Cloud-hosted API for seamless integration

### 💬 Feedback & Contributions
If you’re interested in our project or have any suggestions, please feel free to leave an issue on GitHub or reach out via email.
Thank you for your interest and support!

---

## 🚀 Getting Started

### Project Structure
```bash
Cleanroom-RAG/
│
├── app.py                             # 页面搭建——Streamlit 主入口
├── requirements.txt                   # 依赖列表
├── data                               # 原始数据库
├── scripts/                           # 向量库元数据相对路径修正（即将移除）
├── core/                              # 核心代码
│   ├── utils/                         # 文件读取
│   ├── Embeddings/                    # 文本嵌入
│   ├── VetorBase/                     # 配置本地向量数据库
│   ├── img_storage_prepare/           # 图片数据向量化函数
│   ├── text_storage_prepare/          # 文本数据向量化函数
│   ├── img_storage_update/            # 更新（删减）图片数据库
│   ├── storage_prepare/               # 数据库准备
│   ├── LLM/                           # LLM配置模块
│   ├── Multimodel_LLM/                # 多模态（文本+图片）检索生成
│   ├── Local_ChatLLM/                 # 本地简单测试
│   └── config.py                      # 地址配置文件
└── .env/                              # api_key本地配置（非必须）
```
### Prerequisites
- Python 3.9+

### Installation
```bash
git clone https://github.com/BEEE/Cleanroom-RAG.git
cd Cleanroom-RAG
pip install -r requirements.txt
```

### Usage
```bash
streamlit run app.py
```
This will launch the Cleanroom Design Assistant in your default web browser.
