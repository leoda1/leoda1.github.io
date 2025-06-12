---
title: 关于我
date: 2025-01-28
type: "about"
layout: "about"
---

# 🚀 AI Infra 学习框架  
AI Infra 是支持 AI 模型从开发到生产的重要基础设施。以下是一个完整的 AI Infra 学习框架，覆盖从模型训练到推理、部署和运维的全流程，帮助你在 AI Infra 领域建立完整的知识体系。  

---

## 🎯 1. 能力模型  

| 技能方向 | 目标 | 基础 (超越外行) | 进阶 (超越内行) |
| --- | --- | --- | --- |
| **工具性学习** | 学习 AI 模型训练和开发工具 | - 熟练掌握常见机器学习算法和公式推导<br>- 掌握 TensorFlow/PyTorch/Keras 的 API 使用 | - 深入理解模型结构与内存/显存占用<br>- 掌握 SOTA（State Of The Art）模型 |
| **模型表达** | 通过框架搭建模型 | - 熟练使用 TensorFlow, PyTorch, Keras 建立模型<br>- 掌握 PaddlePaddle 基本用法 | - 能够在实际项目中优化模型结构<br>- 在 Kaggle 或阿里天池等竞赛中获得排名 |
| **模型训练** | 训练与优化模型 | - 熟悉分布式训练架构 (Megatron-LM, DeepSpeed)<br>- 理解多机多卡的训练架构 | - 设计与实现分布式训练系统<br>- 改进训练框架 |
| **模型导出** | 将模型保存并导出 | - 熟悉 ONNX, TensorRT, SavedModel 格式 | - 可自主开发模型导出工具<br>- 掌握跨平台格式转换 |
| **模型部署** | 将模型在生产环境中部署 | - 熟悉 Docker, K8S, 云原生平台<br>- 熟悉流式/在线训练部署 | - 设计高效的模型部署架构<br>- 能够实现快速跨平台部署 |
| **模型推理** | 优化推理性能 | - 掌握 TensorRT, ONNX Runtime, Triton | - 自主开发推理引擎或对现有引擎优化 |
| **模型运维** | 持续优化和监控 | - 熟悉 MLOps 基本流程<br>- 能对模型进行监控与告警 | - 自主研发 MLOps 工具链<br>- 优化大规模模型运维策略 |

---

## 🎯 2. 推理引擎  

推理引擎是将训练好的 AI 模型高效地运行在生产环境中的核心组件，主要涉及以下关键技术：  

| 技术方向 | 说明 |
| --- | --- |
| **计算图优化** | 通过算子融合、常量折叠等手段优化计算图结构 |
| **算子优化** | 针对不同硬件优化算子（CPU、GPU、TPU） |
| **数据排布优化** | 使用 NHWC/NCHW 格式提高访存效率 |
| **量化** | 将浮点计算转换为 INT8/FP16，减少计算开销 |
| **动态批处理** | 允许多个请求合并，提高吞吐量 |
| **缓存优化** | 复用中间计算结果，减少内存占用 |

✅ 常见推理引擎：  
- **TensorRT**（NVIDIA GPU）  
- **ONNX Runtime**（CPU, GPU, FPGA）  
- **TVM**（支持多种 AI 硬件）  
- **OpenVINO**（Intel）  
- **TFLite**（移动端）  

---

## 🎯 3. AI 编译器  

AI 编译器负责将神经网络模型转换为底层硬件代码，涉及的核心技术包括：  

| 组件 | 说明 |
| --- | --- |
| **前端解析** | 解析 PyTorch, TensorFlow, ONNX 等模型格式 |
| **优化** | 自动算子融合、常量折叠、低精度计算 |
| **代码生成** | 针对不同硬件生成汇编或中间代码 |
| **后端** | 调用目标硬件（CUDA, ROCm, OpenCL） |

✅ 代表性 AI 编译器：  
- **TVM**（通用 AI 编译器）  
- **XLA**（TensorFlow 专用）  
- **MLIR**（LLVM 项目）  
- **Glow**（Facebook 专用）  

---

## 🎯 4. 模型存储和导出  

AI 模型需要在不同场景和平台中存储和加载，常见的格式包括：  

| 格式 | 说明 |
| --- | --- |
| **ONNX** | 通用深度学习模型存储格式 |
| **SavedModel** | TensorFlow 原生格式 |
| **TorchScript** | PyTorch 导出格式 |
| **TensorRT** | NVIDIA 优化后的推理格式 |

---

## 🎯 5. 部署和推理优化  

AI 模型部署和推理涉及多个方面的优化工作：  

✅ **推理优化方向**  
- 量化、蒸馏、剪枝、低秩分解  
- 数据布局优化  
- 内存优化  

✅ **部署策略**  
- 通过 Docker/K8S 部署  
- 动态负载均衡  
- A/B 测试  

---

## 🎯 6. MLOps 与持续集成  

MLOps 是 AI 模型在生产环境中的自动化流程，包括：  
- **模型监控**（监控模型精度、性能、成本）  
- **持续集成/部署（CI/CD）**  
- **故障恢复与自动扩容**  
- **版本管理与模型回滚**  

✅ 常见工具：  
- **Kubernetes**（K8S）  
- **MLflow**  
- **TensorBoard**  

---

## 🚀 7. 相关学习资源  

| 资源 | 链接 |
| --- | --- |
| 李宏毅 机器学习 | [Bilibili](https://www.bilibili.com/video/BV1Wv411h7kN) |
| 吴恩达 深度学习 | [Bilibili](https://www.bilibili.com/video/BV1FT4y1E74V) |
| 林轩田 机器学习基石 | [Bilibili](https://www.bilibili.com/video/BV1Cx411i7op) |
| PyTorch 中文教程 | [GitHub](https://github.com/INTERMT/Awesome-PyTorch-Chinese) |
| TensorFlow 官方教程 | [Docs](https://tensorflow.org) |

---

## 🌟 总结  
- ✅ 掌握 AI 模型的开发、训练、导出、部署与推理全流程  
- ✅ 熟悉 TensorFlow、PyTorch、ONNX 等主流框架  
- ✅ 熟悉 TVM、XLA、TensorRT 等编译器和推理引擎  
- ✅ 建立 MLOps 工作流，自动化 AI 模型在生产环境中的迭代  

---

🔥 **AI Infra 是未来 AI 发展的核心方向！开始你的学习之旅吧！** 😎

## ❤️ 如果你觉得内容对你有帮助，可以请我喝一杯咖啡！ 😎
<div style="display: flex; justify-content: center; align-items: center;">
  <div style="margin-right: 20px;">
    <img src="/images/alipay.jpg" alt="支付宝" width="300" height="auto">
  </div>
  <div>
    <img src="/images/wechat.jpg" alt="微信" width="300" height="auto">
  </div>
</div>