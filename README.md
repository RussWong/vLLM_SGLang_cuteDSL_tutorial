# vLLM_SGLang_cuteDSL_tutorial

本仓库主要介绍vLLM, SGLang, cuteDSL等（更多待补充）领域相关知识，你可以明显看出，主要针对大模型推理引擎和Kernel Python DSL。

现今，最流行的开源大模型推理引擎依然是vLLM和SGLang，希望本仓库的jupyter notebook和一些python+cpp代码能帮助大家更好地使用和学习vLLM和SGLang。

另外，Kernel Python DSL是当今流行的kernel开发模式（agent除外），降低了传统高性能Kernel开发的门槛，其中，以cuteDSL为代表，cute cutlass一直是大家头疼的算子库项目，cuteDSL使得更多人都可以参与进来，探索cute layout algebra的乐趣，Enjoy！

## vLLM notebook
相关练习代码采用python语言，以notebook形式呈现，帮助读者快速了解或掌握相关内容。

| 📓 Notebook 链接 | 🧠 Notebook 主要内容 | 🧩 难度等级 | ⭐ 难度 |
|---|---|---|---|
| [vllm_local_single_gpu_quickstart.ipynb](./vllm/vllm_local_single_gpu_quickstart.ipynb) | vLLM 单卡本地快速部署，一行命令启动 OpenAI 兼容服务并完成最小 API 调用闭环。 | 入门 | ⭐⭐ |
| [vllm_multi_turn_memory_minimal_demo.ipynb](./vllm/vllm_multi_turn_memory_minimal_demo.ipynb) | vLLM 多轮对话历史记忆实践，展示 `messages` 维护与最小历史裁剪策略。 | 入门-中级 | ⭐⭐⭐ |

## SGLang notebook
相关练习代码采用python语言，以notebook形式呈现，帮助读者快速了解或掌握相关内容。

| 📓 Notebook 链接 | 🧠 Notebook 主要内容 | 🧩 难度等级 | ⭐ 难度 |
|---|---|---|---|
| [sglang_async_generate_minimal_demo.ipynb](./sglang/sglang_async_generate_minimal_demo.ipynb) | SGLang 异步并发入门，演示 `engine.async_generate(...)` 与 `asyncio.gather(...)` 的最小并发调用流程。 | 入门 | ⭐⭐ |
| [sglang_attention_backend_knobs_minimal_demo.ipynb](./sglang/sglang_attention_backend_knobs_minimal_demo.ipynb) | SGLang 注意力后端参数入门，比较统一后端与 prefill/decode 分离后端配置，并包含自动回退思路。 | 中级 | ⭐⭐⭐ |

## cuteDSL

TODO

## 历史学习文章导航

| 📝 文章链接 | 🧭 类别 | ⭐ 难度 |
|---|---|---|
| [C++模板推导再炫技：统一CUDA elementwise kernel的调用接口](https://zhuanlan.zhihu.com/p/690238529) | C++ | ⭐⭐⭐⭐ |
| [C++模板推导再炫技：统一深度学习框架和推理引擎的各个device各个kernel的调用](https://zhuanlan.zhihu.com/p/688135917) | C++ | ⭐⭐⭐⭐ |
| [一起赏析PaddlePaddle KernelCall源码的C++模板“ 炫技 ”show](https://zhuanlan.zhihu.com/p/669082666) | C++ | ⭐⭐⭐⭐ |
| [CUDA内存分配之cudaMalloc/cudaMallocManaged/cudaMallocAsync详解](https://zhuanlan.zhihu.com/p/2018659595833352770) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [一张图讲清楚Flash Attention 4](https://zhuanlan.zhihu.com/p/2023058994810339447) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [深入解析FlashAttention-V3之Hopper GPU版创新设计 (上篇)](https://zhuanlan.zhihu.com/p/1893400718767022731) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [GPU推理的系统级别优化case(三)-完结篇-推理优化不止算子](https://zhuanlan.zhihu.com/p/31907482356) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [GPU推理的系统级别优化case(二)-推理优化不止算子](https://zhuanlan.zhihu.com/p/30185578082) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [GPU推理的系统级别优化case(一)-推理优化不止算子](https://zhuanlan.zhihu.com/p/29281761483) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [窥FaceBook数据中心AI模型特点, 浅品性能优化和HW-SW co-design](https://zhuanlan.zhihu.com/p/710280932) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [全面探究GPU SM内CUDA core-Tensor core能否同时计算？(下篇)](https://zhuanlan.zhihu.com/p/698572611) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [全面探究英伟达GPU SM内CUDA core-Tensor core能否同时计算？(上篇)](https://zhuanlan.zhihu.com/p/697000619) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [记录Flash Attention2-对1在GPU并行性和计算量上的一些小优化](https://zhuanlan.zhihu.com/p/650947918) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [Paper阅读笔记: Welder: Scheduling Deep Learning Memory Access via Tile-graph](https://zhuanlan.zhihu.com/p/643155184) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [CUDA实现transpose kernel(上)--实现篇](https://zhuanlan.zhihu.com/p/640439125) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [CUDA实现dropout kernel(下）--优化篇](https://zhuanlan.zhihu.com/p/636930189) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [CUDA实现dropout kernel(上）--实现篇](https://zhuanlan.zhihu.com/p/633914118) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [论文阅读笔记-非线性神经网络训练的动态GPU显存节约技术](https://zhuanlan.zhihu.com/p/627042528) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [深入解析cutlass的诞生历程、特性和对友商的各大优势](https://zhuanlan.zhihu.com/p/19597653264) | GPU架构/CUDA | ⭐⭐⭐⭐ |
| [NVIDIA AVO自主进化kernel agent是不是在吹牛？我们真要失业了？](https://zhuanlan.zhihu.com/p/2020562937241159408) | agent | ⭐⭐⭐⭐⭐ |
| [Triton/CUDA Kernel 生成新范式：全链路闭环高性能Kernel Agent架构深入解析](https://zhuanlan.zhihu.com/p/2000176350259086387) | agent | ⭐⭐⭐⭐⭐ |
| [只有V100？小白也能上手的AI推理优化实战方向全解析](https://zhuanlan.zhihu.com/p/2004551809893692210) | 推理引擎 | ⭐⭐⭐ |
| [Dify/ComfyUI沉迷记--一个 AI infra推理加速工程师的跨界探索](https://zhuanlan.zhihu.com/p/1991824416812860189) | 推理引擎 | ⭐⭐⭐ |
| [step3 AF分离推理系统 vs. deepseek EP推理系统，谁更好？](https://zhuanlan.zhihu.com/p/1935665533891633936) | 推理引擎 | ⭐⭐⭐ |
| [手把手教你基于vllm大模型推理框架部署Qwen3-MoE](https://zhuanlan.zhihu.com/p/1902835927396652806) | 推理引擎 | ⭐⭐⭐ |
| [Deep dive vLLM和SGLang推理框架的CPU开销](https://zhuanlan.zhihu.com/p/12201991762) | 推理引擎 | ⭐⭐⭐ |
| [漫谈TensorRT-LLM的关键技术 (未完待续)](https://zhuanlan.zhihu.com/p/917457226) | 推理引擎 | ⭐⭐⭐ |
| [深入分析kimi推理系统Mooncake解决的是什么问题](https://zhuanlan.zhihu.com/p/710706218) | 推理引擎 | ⭐⭐⭐ |
| [全网首篇从tensorRT-LLM MoE CUDA kernel角度理解Mixtral-8x7b的推理加速及展望](https://zhuanlan.zhihu.com/p/691549433) | 推理引擎 | ⭐⭐⭐ |
| [深度解析streamingLLM之无限长文本生成能力](https://zhuanlan.zhihu.com/p/675626163) | 推理引擎 | ⭐⭐⭐ |
| [大模型文本生成策略：搜索or采样？这很难选 (搜索篇)](https://zhuanlan.zhihu.com/p/664027520) | 推理引擎 | ⭐⭐⭐ |
| [从AI推理优化角度看LLaMA的模型结构和源码](https://zhuanlan.zhihu.com/p/661347348) | 推理引擎 | ⭐⭐⭐ |
| [CUDA PagedAttention kernel源码解析--大模型推理服务框架vLLM要点简析（下）](https://zhuanlan.zhihu.com/p/658233994) | 推理引擎 | ⭐⭐⭐ |
| [PagedAttention--大模型推理服务框架vLLM要点简析 (中)](https://zhuanlan.zhihu.com/p/655561941) | 推理引擎 | ⭐⭐⭐ |
| [大模型推理服务框架vLLM要点简析 (上)](https://zhuanlan.zhihu.com/p/654259045) | 推理引擎 | ⭐⭐⭐ |
| [一张图讲清楚Flash Attention 4](https://zhuanlan.zhihu.com/p/2023058994810339447) | 算子 | ⭐⭐⭐⭐ |
| [深入解析SageAttention的缺点分析、动机和原理](https://zhuanlan.zhihu.com/p/2011838629220213431) | 算子 | ⭐⭐⭐⭐ |
| [饭前闲聊 GPU 高性能算子编程新势力：老大哥TVM加入cuTile、Tilelang和triton的深度对话 (2)](https://zhuanlan.zhihu.com/p/1982179841932550422) | 算子 | ⭐⭐⭐⭐ |
| [饭后闲聊 GPU 高性能算子编程新势力：cuTile、Triton 与 TileLang 的深度对话 (1)](https://zhuanlan.zhihu.com/p/1981042493769413822) | 算子 | ⭐⭐⭐⭐ |
| [深入解析FlashAttention-V3之FP8/FP16/BF16关键细节实现 (下篇)](https://zhuanlan.zhihu.com/p/1898427919497398192) | 算子 | ⭐⭐⭐⭐ |
| [深度解析DeepSeek NSA原生稀疏注意力idea和kernel](https://zhuanlan.zhihu.com/p/26319386548) | 算子 | ⭐⭐⭐⭐ |
| [下游训练任务起飞！FlashAttention终于高性能地支持多样的attention mask！](https://zhuanlan.zhihu.com/p/7793258241) | 算子 | ⭐⭐⭐⭐ |
| [AI高性能优化：ResNet50静态图优化手段之Pad+Conv2d的融合](https://zhuanlan.zhihu.com/p/682981283) | 算子 | ⭐⭐⭐⭐ |
| [(代码实战) AI算子开发必备之高维坐标和一维内存偏移的互相转换类IndexOffsetHelper](https://zhuanlan.zhihu.com/p/677914346) | 算子 | ⭐⭐⭐⭐ |
| [深度解析Group Query Attention(GQA)为什么能给LLM decoder带来极大推理加速](https://zhuanlan.zhihu.com/p/667259791) | 算子 | ⭐⭐⭐⭐ |
| [记录Flash Attention1-加速标准注意力的计算利器](https://zhuanlan.zhihu.com/p/650912253) | 算子 | ⭐⭐⭐⭐ |
| [ParallelKittens: 使用ThunderKittens也可以轻松开发计算/通信overlapped kernel啦](https://zhuanlan.zhihu.com/p/1997011080858343138) | 通信 | ⭐⭐⭐⭐⭐ |
| [全面解析MoE专家并行EP all-to-all Pytorch算子(小白也能看懂)](https://zhuanlan.zhihu.com/p/1967192540953425479) | 通信 | ⭐⭐⭐⭐⭐ |
| [大模型通信算子--int8/int4 custom AllReduce kernel的动机、挑战和设计](https://zhuanlan.zhihu.com/p/1960086916654407812) | 通信 | ⭐⭐⭐⭐⭐ |
| [大模型计算/通信overlapped kernel(二)--AllGather+Gemm/Gemm+ReduceScatter](https://zhuanlan.zhihu.com/p/1948749443802313796) | 通信 | ⭐⭐⭐⭐⭐ |
| [大模型计算/通信overlapped kernel(一)--动机和概念](https://zhuanlan.zhihu.com/p/1930681680127047148) | 通信 | ⭐⭐⭐⭐⭐ |
| [SageAttention3(上)-首个FP4 attention算子推理解决方案](https://zhuanlan.zhihu.com/p/2019842447191069623) | 量化 | ⭐⭐⭐⭐ |
| [SageAttention2-int4/FP8真的有加速作用吗](https://zhuanlan.zhihu.com/p/2012945650954823051) | 量化 | ⭐⭐⭐⭐ |
| [nvFP4 Batch GEMV算子系列(下)--Pytorch+Blackwell协同开发nvFP4 BatchGEMV](https://zhuanlan.zhihu.com/p/1976766248017733187) | 量化 | ⭐⭐⭐⭐ |
| [nvFP4 Batch GEMV算子系列(上)--关于mxFP4/nvFP4知道这些就OK了](https://zhuanlan.zhihu.com/p/1976382945951495795) | 量化 | ⭐⭐⭐⭐ |
| [手把手教你用赤兔大模型推理框架在5090上部署 Qwen3-32B-FP4](https://zhuanlan.zhihu.com/p/1974387560643073803) | 量化 | ⭐⭐⭐⭐ |
| [基于vLLM v1测试BFloat16 vs FP8 Qwen3-MoE模型吞吐性能的重大发现!](https://zhuanlan.zhihu.com/p/1908632663360770832) | 量化 | ⭐⭐⭐⭐ |
| [大模型量化技术祛魅](https://zhuanlan.zhihu.com/p/2994427367) | 量化 | ⭐⭐⭐⭐ |
| [论文阅读－新的AI模型压缩技术：解决大模型LLM的int8精度掉点-SmoothQuant](https://zhuanlan.zhihu.com/p/629834231) | 量化 | ⭐⭐⭐⭐ |
| [全面认识模型压缩技术之稀疏，motivated by混合专家模型MoE LLM的稀疏特性](https://zhuanlan.zhihu.com/p/694339704) | 量化 | ⭐⭐⭐⭐ |
| [记AI-infra/大模型推理社招面试一兄弟的全过程 (v3.0)](https://zhuanlan.zhihu.com/p/1920946738270810330) | 面试 | ⭐⭐ |
| [记年前一次LLM推理优化实习生面试暨解答上文留下的cutlass问题](https://zhuanlan.zhihu.com/p/23109780409) | 面试 | ⭐⭐ |
| [记上周秋招面试一小伙的全过程~](https://zhuanlan.zhihu.com/p/714119085) | 面试 | ⭐⭐ |
| [面试撕leetcode环节的C++ STL常用用法总结（上）](https://zhuanlan.zhihu.com/p/670566463) | 面试 | ⭐⭐ |
| [C++面试高频之单例模式、懒汉模式、饿汉模式](https://zhuanlan.zhihu.com/p/660022573) | 面试 | ⭐⭐ |
| [实习去小公司小厂到底有没有价值？](https://zhuanlan.zhihu.com/p/657302789) | 面试 | ⭐⭐ |
| [我一直想整一篇AI系统/大模型LLM优化领域paper，有哪些可以做的点？发表难度如何？](https://zhuanlan.zhihu.com/p/655879601) | 面试 | ⭐⭐ |
| [AI工程优化+CUDA的面经（基础篇）！](https://zhuanlan.zhihu.com/p/654572960) | 面试 | ⭐⭐ |

## 社区
近期，我创立了一个AI Infra技术讨论社区，正在起步阶段，欢迎对AI Infra技术感兴趣热衷于讨论交流的伙伴加入，目前暂服务 vLLM/SGLang/CUDA/cutlass/kernel agent/kernel human/etc... 等大模型推理引擎的学习者和从业者，希望我能一直运营下去orz。

做这个的原因是想打造垂直、深度、可沉淀的技术交流空间，微信群飞书群都太零碎，想把大家从微信群/飞书群的泛交流，升级为同好者的长期技术成长社区，希望大家一起持续输出高质量内容

### 📚 社群包含什么？
* 🔧 分主题技术频道：vLLM/SGLang/CUDA/cutlass 等细分方向，精准讨论不刷屏
* 📅 固定栏目更新：每周技术热点、hands-on 代码教程、技术深度探讨、Q&A 汇总
* 📚 专属学习资源：教程、论文、代码库、最佳实践一站式获取
* 🎤 线上分享 / 项目交流：后续开放技术演讲、Demo 展示、代码 Review

### 🎯 能帮你解决什么问题？
* 学习中遇到的 vLLM/SGLang 部署、优化、排障问题，随时交流解决
* 系统跟进 AI Infra 最新技术动态，不落后行业节奏
* 找到同频技术伙伴，一起刷题、做项目、共同成长
* 后续对接行业招聘、技术合作等机会

### 👇 加入方式
直接点击链接即可进入：https://kook.vip/MVqLuk
进群后请先查看「新手指南」，期待和大家一起深耕 AI Infra，共同成长！

（注意：社区目前建设在kook，PC端和手机端都可访问，有朋友反映手机端广告较多，建议在PC端访问，我没有遇到任何广告跳转，这个我正在想办法有没有更好的平台支持我去做社区，敬请关注！）

## 关注我

### 知乎

[知乎主页](https://www.zhihu.com/people/russwong)

### 公众号

AI不止算法
