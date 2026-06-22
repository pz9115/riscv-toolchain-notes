# RISC-V Zvdota/Zvbdota 扩展介绍

- 日期: 2026-06
- 讲者: Jiawei Chen
- 主题: RISC-V Zvdota/Zvbdota extension and GNU Toolchain enablement
- 语言: 中文
- 格式: 公开演讲 slides
- Slides: [slides.pdf](./slides.pdf)
- 相关公开草案: [riscv-isa-manual zvbdot branch](https://github.com/riscv/riscv-isa-manual/tree/zvbdot)

## Abstract

本报告介绍 RISC-V Zvdota/Zvbdota 向量点积扩展的背景与设计，并从 GNU Toolchain 支持角度讨论相关 enablement 工作。

内容包括 horizontal dot-product 和 batched dot-product 的基本语义、数据格式、`vtype.altfmt`、`ci` immediate，以及 GNU Binutils 和 GCC 侧的支持方案。Binutils 相关内容包括 `-march`、opcode、operand 和 tests；GCC 相关内容包括 machine pattern、RVV intrinsic 和合法性检查。

## Notes

该 PDF 是公开演讲材料，用于长期记录和后续技术参考。

材料内容反映报告时点的 extension 设计、toolchain 支持方案和 upstream 进展。后续实现或规范细节如有变化，应以公开 specification、upstream patch 和最新工具链代码为准。

Slides are licensed under CC BY-NC-SA 4.0 unless otherwise noted.
