# 来源、阅读范围与设计归属

核查日期：2026-10-29。以下是本 skill 的方法依据与启发，不代表这些机构认可或验证本 skill。
运行 skill 时需重新查询当前研究文献和目标投稿要求，不能把本文件当最新文献库。

## Research-Starter-Kit

- 来源：[LAMDA-NeSy/Research-Starter-Kit](https://github.com/LAMDA-NeSy/Research-Starter-Kit)。
- 已读取仓库 README；核查时主分支提交为 `36ba390d153f5289308ec833e2b633c26b304a7b`。
  [固定版本 README](https://github.com/LAMDA-NeSy/Research-Starter-Kit/blob/36ba390d153f5289308ec833e2b633c26b304a7b/README.md)。
- 已实读下列六篇飞书公开正文。网页工具直接解析失败，改用匿名 HTTP 返回的公开 HTML，
  读取 SSR 文字及内嵌 `block_map/initialAttributedTexts` 并交叉核对。未绕过登录或访问控制。
  阅读范围仅为响应中的文本，不包括图片、附件、评论、历史版本及未列出的其他教程。
- GitHub 元数据在本次核查中未声明 license。这里保留署名与链接，采用原创流程，不复制、翻译或镜像教程正文、图片及代码。
- 本 skill 将入门主题转成“项目证据与决策”的操作流程，不声称是原项目官方版本或完整课程复刻。

实际读取的正文与采用方式：

- [如何做科研？](https://dy8q0bnq8y.feishu.cn/wiki/LfR9woW57iWpQWkRKJhcoFF7ndb)：
  “做研究的基本过程 / Problem / Concrete Work”。采用问题、想法与理论/实验工作的区分，以及有效/失效条件的分析。
- [如何想 Idea？](https://dy8q0bnq8y.feishu.cn/wiki/MxYVwN0lEiv5HUkLEJccRJI3nTd)：
  问题来源与价值判断。采用失败、解释缺口、结论冲突和实际需求作为问题线索；不把方法组合本身当价值证明。
- [如何找论文？](https://dy8q0bnq8y.feishu.cn/wiki/Co5awLsRiiuYAlkqHhCcwGBanub)：
  种子论文、文献网络、代码/基准生态。采用前后向追踪及近邻设定核对；具体 venue 名单不作为价值评级。
- [如何读论文？](https://dy8q0bnq8y.feishu.cn/wiki/Ow8fw2HtEiixDgkWlkbckdvHnef)：
  问题、已有工作、实验与读后思考。采用问题到证据的重建与关键近邻核验；不硬编码经验性阅读时间比例。
- [一些好的习惯](https://dy8q0bnq8y.feishu.cn/wiki/Bp2AwrSnAiGaH2khJaqczVXznwc)：
  实验日志与尽早验证。采用记录假设、配置、失败和最小验证；具体预算及停止阈值另由项目确定。
- [如何写论文—Experiments](https://dy8q0bnq8y.feishu.cn/wiki/KHgSw2MkrikxlskGe5qclkdbn2c)：
  实验设置、主结果、消融、分析及异常结果。采用贡献到证据的映射、公平比较和边界检查。
  不采纳淡化异常影响的修辞目标：本 skill 要求如实报告异常、效应、不确定性及其对结论的影响。

补充阅读了 README 链接的 [pengsida/learning_research](https://github.com/pengsida/learning_research)
之 README、`getting_started_in_research.md` 与 `getting_advanced_in_research.md`。
其具体培养路径来自作者实验室和计算机视觉/ML经验，不作为跨学科统一门槛；受限 Notion 页面不算已读。

## 直接读取的方法依据

### M1：DARPA 的研究规划问题

[The Heilmeier Catechism](https://www.darpa.mil/about/heilmeier-catechism)，官方正文。
启发：明确目标、现有做法局限、方案差异、潜在价值、风险、资源与阶段检验。
适用：问题定义与可行性。边界：这些问题不能证明新颖性或预测发表水平。

### M2：PRISMA-S 检索报告

Rethlefsen et al., *PRISMA-S: an extension to the PRISMA Statement for Reporting Literature Searches in Systematic Reviews*。
[原始全文 PDF](https://jmla.pitt.edu/ojs/jmla/article/view/962/1274)；[官方入口](https://www.prisma-statement.org/prisma-search)。
已读原始全文，重点为检索报告条目。
采用：记录来源/平台、完整检索式、日期、限制、引文追踪与去重。
边界：这是系统综述的检索报告规范，本 skill 只借鉴透明记录原则；普通诊断不自动满足系统综述要求。

### M3：NeurIPS 实证与理论报告

[NeurIPS Paper Checklist Guidelines](https://neurips.cc/public/guides/PaperChecklist)，官方正文。
采用：主张与证据相称，数据划分、模型选择、复现、资源与误差来源需可解释。
边界：ML 投稿背景；不推广成所有学科都要固定运行次数或开放全部数据，具体投稿以当年规则为准。

### M4：机器学习比较中的变异

Bouthillier et al., *Accounting for Variance in Machine Learning Benchmarks*, MLSys 2021。
[原始论文 PDF](https://proceedings.mlsys.org/paper_files/paper/2021/file/0184b0cd3cfb185989f858a1d9f5c1eb-Paper.pdf)，已读全文。
采用：考虑采样、初始化、增强与超参数等变异来源，不以单次最好值推断稳定优势。
边界：不同研究设计应选相应分析单位和估计方法，不机械复制一种判据到所有问题。

### M5：数据泄漏与科学主张

Kapoor & Narayanan, *Leakage and the reproducibility crisis in machine-learning-based science*, Patterns 2023。
[正式版 DOI](https://doi.org/10.1016/j.patter.2023.100804)；[预印本全文](https://arxiv.org/pdf/2207.07048)。
已读预印本全文，正式版元数据通过 PubMed/PMC 记录核实；出版社直连受限，不声称已读正式版全文。
采用：训练/测试隔离、预处理、实体/时间相关性、预测时可得信息以及测试分布与主张的一致性。
边界：预测性能不能独立证明因果机制；潜在污染和已经确认的泄漏需区分。

### M6：内容导向的研究评价

[DORA：San Francisco Declaration on Research Assessment](https://sfdora.org/read/)，官方正文。
采用：按实际研究内容和贡献评价，承认数据、软件等产出，不用期刊影响因子替代判断。
边界：DORA 没有提供本 skill 的阶段划分、创新评级或录用概率。

### M7：调参预算的可比性

Sivaprasad et al., *Optimizer Benchmarking Needs to Account for Hyperparameter Tuning*, ICML 2020。
[PMLR 原始记录与摘要](https://proceedings.mlr.press/v119/sivaprasad20a.html)，已读官方摘要并核实元数据。
采用：比较时考虑调参与优化预算，而不只最终最好分数。
边界：本次未据全文抽取具体实现或声称某个优化器普适最优。

## 格式依据

[OpenAI 官方 Build skills](https://developers.openai.com/plugins/build/skills)：SKILL.md 的名称/描述、
指令与按需参考文件结构。此来源只用于技能包装，不是科研判断的依据。

## 本项目原创的操作设计

- C/E/P/G/R/T 的追溯关系、S0–S5 关口、创新与证据的双轴描述。
- 六维诊断、优先级 Q0–Q3、继续/修正/收窄/转向/停止的决策分支。
- 三路文献搜索和“缺口—机制—论文—迁移—修改—区分验证”建议链条。
- 项目快照、报告字段、跨周期更新和行为演练案例。

这些设计是依据上述资料形成的工作框架，尚未经过正式测量学验证或长期效果研究。
“较强”“受控支持”等词是可解释的操作标签，不代表客观量化创新分数。
外部论文与教程的版权和许可仍属于各自权利人；本仓库不再分发其全文。
