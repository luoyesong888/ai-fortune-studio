# 玄星命理实验室 · AI Fortune Studio

一个“排盘引擎负责准确计算、AI 只负责解释”的命理产品 MVP。当前已接入 `lunar-typescript` 与 `iztro`，并为 Kerykeion 西洋占星服务预留产品入口。

## 功能

- 生辰信息输入与响应式产品界面
- 八字四柱、农历信息、五行显性分布
- 紫微斗数排盘引擎调用与状态展示
- 西洋占星 Kerykeion 服务接口设计
- 综合解读、娱乐用途边界说明

## 本地运行

```bash
npm install
npm run dev
```

生产构建：`npm run build`

## 技术架构

浏览器端使用 React + TypeScript + Vite。`lunar-typescript` 负责历法和八字，`iztro` 负责紫微斗数。正式版本建议新增 FastAPI 服务封装 Kerykeion，并将三种引擎统一为结构化 JSON 后交给模型解读。

## 商业化提醒

Kerykeion 使用 AGPL-3.0；闭源商业化前需进行许可证评估。其他依赖也应以项目当前 LICENSE 为准重新核验。

## 免责声明

本项目用于传统文化研究、产品原型与娱乐体验，不构成医疗、法律、投资或人生重大决策建议。
