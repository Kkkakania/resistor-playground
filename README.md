# ⚡ Resistor Playground · 电阻色环游乐场

> 读色环、反查色环、限时闯关——一个写给电类同学的零依赖网页小工具。
> Decode, encode and gamify resistor color bands — a zero-dependency web toy for EE students.

[![Pages](https://img.shields.io/badge/demo-GitHub%20Pages-34d399)](https://kkkakania.github.io/resistor-playground/)
[![License: MIT](https://img.shields.io/badge/license-MIT-38bdf8.svg)](LICENSE)
![No dependencies](https://img.shields.io/badge/dependencies-0-c9a227)

单个 `index.html`，没有任何依赖，双击即可打开，也可一键挂到 GitHub Pages。
A single `index.html` with no build step and no dependencies — open it directly or host it on GitHub Pages.

## ✨ 功能 Features

- **🎨 解码 Decode** — 选择每一环的颜色，电阻图实时更新，自动算出阻值、容差和实际范围。支持 4 环 / 5 环。
- **🔢 反查 Encode** — 输入目标阻值（Ω / kΩ / MΩ）和容差，自动给出对应色环。
- **🎮 闯关 Quiz** — 随机出题、四选一、连击计分 + 10 秒倒计时，专治"色环记不住"。
- **🌗 实验室深色主题**，响应式，手机也能玩；颜色对照表常驻底部。

## 🚀 在线体验 Live Demo

部署后访问：**https://kkkakania.github.io/resistor-playground/**

## 🖥️ 本地运行 Run Locally

```bash
git clone https://github.com/Kkkakania/resistor-playground.git
cd resistor-playground
# 直接用浏览器打开 index.html 即可；或起一个本地服务：
python3 -m http.server 8000   # 然后访问 http://localhost:8000
```

## 🎨 色环对照表 Color Code Reference

| 颜色 Color | 数字 Digit | 倍率 Multiplier | 容差 Tolerance |
|---|---|---|---|
| 黑 Black | 0 | ×1 | — |
| 棕 Brown | 1 | ×10 | ±1% |
| 红 Red | 2 | ×100 | ±2% |
| 橙 Orange | 3 | ×1k | — |
| 黄 Yellow | 4 | ×10k | — |
| 绿 Green | 5 | ×100k | ±0.5% |
| 蓝 Blue | 6 | ×1M | ±0.25% |
| 紫 Violet | 7 | ×10M | ±0.1% |
| 灰 Grey | 8 | ×100M | ±0.05% |
| 白 White | 9 | ×1G | — |
| 金 Gold | — | ×0.1 | ±5% |
| 银 Silver | — | ×0.01 | ±10% |

> 数据依据 IEC 60062 电阻色环标准。Data based on the IEC 60062 standard.

**口诀小抄**：棕红橙黄绿，蓝紫灰白黑——对应 1 2 3 4 5、6 7 8 9 0。

## 🛠️ 技术 Tech

纯 HTML + CSS + 原生 JavaScript，电阻用内联 SVG 绘制，无外部库、无网络请求。
Plain HTML + CSS + vanilla JS; the resistor is drawn with inline SVG. No libraries, no network calls.

## 📄 License

[MIT](LICENSE) © 2026
