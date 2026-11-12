# 皇极经世 · huangji core

皇极元会运世纪年。本仓从 [知几排盘](https://github.com/weihaoyang/qimen-llm-chart) 提取 TypeScript 源码及对应测试，可独立安装依赖并运行；支持 ESM、CommonJS 与 TypeScript。

## 运行

需要 Node.js 20 或更高版本。

```sh
npm install
npm test
npm run typecheck
```

发布后安装：`npm install @singseq/huangji-core`。入口 `@singseq/huangji-core`；其他模块可按 `@singseq/huangji-core/模块名` 导入。源码与测试位于 `src/`。

## 资料与案例

- [原项目研究论文](https://github.com/weihaoyang/qimen-llm-chart/blob/main/docs/research/calculation-audit-paper.md)
- [原项目来源及技术说明](https://zh.wikisource.org/wiki/皇極經世書)

- reproduces three dated entries in Huangji Jingshi volume four（`src/chronology.test.ts`）
- anchors the epoch at 公元前 67017 = 甲子（`src/chronology.test.ts`）
- matches the two historical anchors from the spec（`src/chronology.test.ts`）
- positions 公元 2026 across every level（`src/chronology.test.ts`）
- converts historical years and rejects 公元 0 年（`src/chronology.test.ts`）

这些案例验证列出的计算或文本字段，不代表预测效果经过验证。对于现代知识或几何构造，资料链接标注其实际来源，不冒称古籍。

## 授权

本仓代码按 [GPL-3.0-only](LICENSE) 发布，源自知几排盘。

- 来源：[https://github.com/Ryanlyly-ai/huangji-jingshi](https://github.com/Ryanlyly-ai/huangji-jingshi)；许可原文：[`huangji-jingshi-MIT.txt`](LICENSES/huangji-jingshi-MIT.txt).

外部资料和影像按各自来源的使用条件处理，本仓不附古籍影像。
