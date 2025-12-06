# 👋 **Hello, I'm Leandro Cunha**

## 💡 **Senior Applied AI/ML Engineer | LLM Systems & Production Architecture**  

I am a Senior Engineer specializing in production-grade Applied AI , ML and Data engineering.  With 16+ years of engineering experience in mission-critical high-availability systems sectors like Power Grids, Pharma, and Aeronautics. I hold an M.Sc. in AI (Distinction), and I aim to build efficient solutions with modern Deep Learning that perform fast and reliably in the real world.

---

## 🚀 **Core Competencies**

- **AI & Agentic Systems**: **PyTorch**, **LLM Architectures** (RAG, Multi-Agent Systems/CrewAI), LangChain, Computer Vision (OpenCV, OpenVino), Explainable AI.
- **Production MLOps**: **Kubernetes**, **Docker**, **Infrastructure as Code (Terraform, AWS CDK)**, Pipeline Orchestration (Airflow, Dagster, Kedro).
- **Data Engineering at Scale**: **PySpark**, **Databricks**, Distributed Processing, Data Warehousing (BigQuery, Redshift).
- **Languages**: Python (Expert), JavaScript (React/Node.js).

---

## 📂 **Featured Projects**

---

### 1. **Game Analytics Platform**  
*Production-grade analytics dashboard with full-stack deployment*

- Kubernetes-ready analytics platform for large-scale game metrics (ETL → API → UI)  
- **Tech**: FastAPI, React/TypeScript, Polars, Docker, Kubernetes, CI/CD  
- **Key Features**:
  - ETL pipeline: CSV → Parquet (50-70% memory savings vs. pandas)
  - Real-time metrics aggregation and filtering
  - Kubernetes deployment (Kind for local testing)
  - Calibration factor updates via API
  - Scalable architecture ready for production clouds
- 👉 [`game_analytics` repo](https://github.com/leovcunha/game_analytics)

---

### 2. **Movie Recommendation Engine**  
*Collaborative filtering system handling 1M+ user ratings with advanced memory optimization*

- Hybrid recommendation system (user-based + item-based collaborative filtering)  
- - **Tech**: FastAPI, React, Scipy (sparse matrices), TMDB API, Caching  
- **Key Features**:
  - Hybrid approach: 40% user-based + 60% item-based predictions
  - **Memory optimization**: Dynamic loading based on available RAM, sparse matrices, batch processing (1000-user batches)
  - Cold-start solution: TMDB API integration with intelligent fallback
  - Handles datasets with 1M+ user ratings on resource-constrained machines
  - Model caching for fast inference
- 👉 [`movie-recom` repo](https://github.com/leovcunha/movie-recom)

---

### 3. **Deepfake Detection with CNN+RNN**  
*M.Sc. thesis: Hybrid CNN-RNN architectures for deepfake video detection*

- Deep learning system for detecting forged videos using EfficientNet (CNN) and EfficientNet-GRU (Hybrid)   
- **Tech**: PyTorch, EfficientNet, GRU, Particle Swarm Optimization, Video Processing  
- **Key Features**:
  - Datasets: DFDC (deepfakes), CelebDF-v2 (deepfakes), YouTube Faces (real)
  - Hyperparameter tuning: Manual search + PSO (Particle Swarm Optimization)
  - Architecture comparison: Pure CNN vs. Hybrid CNN-RNN
  - Finetuned model weights available
  - Comprehensive experiment notebooks (data analysis → preliminary → tuning → final testing)
- 👉 [`deepfake_detection_cnn_rnn` repo](https://github.com/leovcunha/deepfake_detection_cnn_rnn)

---

### 4. **ML Algorithms from Scratch**  
*Classical machine learning from first principles in NumPy*

- 10+ algorithms implemented entirely from scratch (KNN, Logistic Regression, Random Forest, SVM, MLP, PCA, Clustering, etc.)  
- **Tech**: Python, NumPy, Unit Tests, Visualizations  
- **Key Features**: Decision boundary plots, example scripts, comprehensive tests  
- 👉 [`ML-Algorithms-from-Scratch` repo](https://github.com/leovcunha/ML-Algorithms-from-Scratch)
---

### 5. **Real-Time Gaze-Based Mouse Control**  
*Computer vision pipeline optimized for edge deployment*

- Real-time eye-tracking system that controls mouse pointer based on gaze direction  
- **Tech**: Intel OpenVINO, OpenCV, Python, Model Precision Optimization  
- **Key Features**:
  - Multi-stage pipeline: Face Detection → Facial Landmarks → Head Pose → Gaze Estimation
  - Edge-optimized: Benchmarks for FP32, FP16, FP16-INT8 (precision/speed/size trade-offs)
  - Performance analysis: Loading times & inference times per stage
  - Practical insights: precision selection based on hardware constraints
- 👉 [`mouse_pointer_controller` repo](https://github.com/leovcunha/mouse_pointer_controller)

---

## 🌐 **Let's Connect**

- **LinkedIn**: [Leandro Cunha](https://www.linkedin.com/in/leandro-vcunha/)  

