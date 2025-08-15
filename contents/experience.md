### 经历与项目  |  Experience & Projects  

---

#### 1. 半监督医学图像分割——从想法到 CCF-B 论文  
**2023.07 – 2024.05**  
- 提出一种将基础模型特征与传统 CNN 耦合的标注高效框架，用于心脏 CT 分割。  
- 设计双头一致性损失 + 置信度伪标签模块，标注成本较全监督降低 **65 %**。  
- 在 ACDC & MM-WHS 数据集上验证；成果发表于 **ICASSP 2025 (CCF-B)**，代码开源并获 200+ Star。

**Semi-supervised Medical Image Segmentation — From Idea to CCF-B Paper**  
**Jul 2023 – May 2024**  
- Proposed a label-efficient framework coupling foundation-model features with classical CNNs for cardiac CT segmentation.  
- Introduced dual-head consistency loss & confidence-based pseudo-labeling, cutting annotation cost by **65 %**.  
- Extensive experiments on **ACDC & MM-WHS**; results accepted to **ICASSP 2025 (CCF-B)**; open-source repo gained **200+ GitHub stars**.

---

#### 2. 端到端 RAG 系统——数据 → 检索 → 生成 → 运维  
**2023.09 – 2024.02**  
- 构建 50 万 + 技术文档的全栈 RAG：  
  – 数据：PDF → 分块 → bge-large-zh 向量化 → Milvus。  
  – 检索：稠密 + BM25 混合 + bge-reranker-large。  
  – 生成：Llama-2-13B + LoRA 微调，BLEU ↑ **12 %**。  
- 基于 K8s+Kubeflow 部署，平均延迟 **< 1.2 s**，日活 2 k+ 查询。

**End-to-End RAG System — Data → Retrieval → Generation → Ops**  
**Sep 2023 – Feb 2024**  
- Built a full-stack RAG on **500k+ technical PDFs**:  
  – **Data**: chunking → bge-large-zh embeddings → Milvus vector store.  
  – **Retrieval**: dense + BM25 hybrid search with bge-reranker-large.  
  – **Generation**: Llama-2-13B fine-tuned with LoRA; **BLEU ↑ 12 %**.  
- Deployed on **K8s+Kubeflow**, auto-scaling HPA, **< 1.2 s** avg latency, serving **2k+ queries/day**.

---

#### 3. RAG 与模型微调——企业实习  
**2024.06 – 至今**  
- 将 RAG 扩展至电信运维手册场景；对 **Qwen-14B** 指令微调 10 万 + 样本，ROUGE-L ↑ **9 %**。  
- 引入 PPO-RLHF，幻觉率从 **18 % → 7 %**。

**RAG & Model Fine-tuning — Industry Internship**  
**Jun 2024 – Present**  
- Extended the above RAG to **telecom manuals**; instruction-tuned **Qwen-14B** on 100k samples; **ROUGE-L ↑ 9 %**.  
- Integrated **PPO-RLHF**; hallucination rate dropped from **18 % → 7 %**.

---

#### 4. K8s + KubeEdge 边云协同  
**2022.11 – 2023.04**  
- 设计基于 KubeEdge 的弹性推理平台，基站 ARM 节点卸载 CNN，云端 CPU 下降 **42 %**。  
- 实现 MQTT + DeviceTwin 实时健康检查与 OTA；**KubeCon China 2023** 学生展示。

**Edge-Cloud Synergy with K8s + KubeEdge**  
**Nov 2022 – Apr 2023**  
- Designed an elastic inference platform using **KubeEdge**; offloaded CNNs to ARM edge nodes, **cloud CPU ↓ 42 %**.  
- Implemented **MQTT + DeviceTwin** health-check & OTA; demo presented at **KubeCon China 2023** student track.

---

#### 5. 小米 CyberDog 2  
**2023.01 – 2023.05**  
- 将 RT-DETR 移植至 Jetson Orin，帧率 30→55 FPS。  
- AprilTag + VIO 融合室内定位，100 m 漂移 **< 2 cm**；向小米开源仓库提交 **2 PR** 已合并。

**Xiaomi CyberDog 2 — Perception & Control**  
**Jan 2023 – May 2023**  
- Ported **RT-DETR** to NVIDIA Jetson Orin, boosting FPS from **30 → 55**.  
- Fused **AprilTag + VIO** for indoor localization; drift **< 2 cm** over 100 m; **2 PRs** merged to Xiaomi repo.

---

#### 6. SAM 国家级大创  
**2023.03 – 2024.03**  
- 基于 **SAM-Medical** 微调 1.5 万张 CT 切片，Dice ↑ **4.7 %**。  
- 开发 PyQt5 一键分割 + 3-D 网格导出软件，已在两家医院试用。

**National Undergraduate Innovation Program on SAM**  
**Mar 2023 – Mar 2024**  
- Fine-tuned **SAM-Medical** on 15k labeled CT slices; Dice ↑ **4.7 %**.  
- Built **PyQt5 GUI** for one-click segmentation & 3-D mesh export; adopted by two hospitals.

---

#### 7. DSL → C++ CNN 编译器  
**2022.02 – 2022.08**  
- 设计描述卷积/池化/注意力的 DSL，并编写 Python→C++ 转译器，生成 **OpenMP+SIMD** 代码，速度提升 **3.8×**。  
- 基于 PEG 解析器 + LLVM-IR 后端，共 1 k 行代码。

**DSL-to-C++ Compiler for Custom CNN Operators**  
**Feb 2022 – Aug 2022**  
- Designed a DSL describing convolutions, pooling, and attention blocks; implemented a **Python→C++ transpiler** generating **OpenMP+SIMD** code, achieving **3.8× speed-up**.  
- Used **PEG parser** & **LLVM-IR** backend; **1k LOC**.

---

#### 8. CUDA 矩阵乘法内核  
**2021.10 – 2021.12**  
- 实现 tiling + shared-memory SGEMM，RTX-3080 上达 **1.7 TFLOPS**（cuBLAS 92 %）。  
- Nsight Compute 调优，共享内存 bank 冲突减少 **64 %**。

**CUDA Matrix Multiplication Kernels**  
**Oct 2021 – Dec 2021**  
- Implemented **tiling + shared-memory SGEMM**, reaching **1.7 TFLOPS** on RTX-3080 (**92 % of cuBLAS**).  
- Profiled with **Nsight Compute**; reduced shared-memory bank conflicts by **64 %**.

---

#### 9. 机器学习 & 大模型课程  
- 完成 **CS336 (Stanford)**：Large Language Models，全部实验 + 参数高效微调期末项目。  
- 自学：Goodfellow《Deep Learning》、Sutton《RL》、Understanding Deep Learning。

**Machine Learning & Large Model Coursework**  
- Completed **CS336 (Stanford)**: Large Language Models — all labs & final project on **parameter-efficient fine-tuning**.  
- Self-studied: *Deep Learning* (Goodfellow), *Reinforcement Learning* (Sutton), *Understanding Deep Learning*.

---

#### 10. 数学自学  
- 完成 14 本研究生级教材：Ahlfors《复分析》、Rudin《泛函分析》、Boyd《凸优化》等。  
- 解决 300+ Putnam & ICPC 题；校数学竞赛前 **3 %**。

**Mathematics Self-Study**  
- Completed **14 graduate-level textbooks**: *Complex Analysis* (Ahlfors), *Functional Analysis* (Rudin), *Convex Optimization* (Boyd), etc.  
- Solved 300+ problems from **Putnam & ICPC** archives; ranked **top 3 %** in university math contest.

