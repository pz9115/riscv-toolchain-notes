# Topics

This file tracks article ideas and technical notes for future writing. Items here are candidates, not published articles.

## RISC-V ISA Extension Enablement

- 如何判断一个 RISC-V 扩展是否需要工具链支持
- RISC-V 扩展工具链支持的几个层次：assembler、disassembler、compiler、testsuite
- 从 ISA extension 到 GNU Toolchain patch 的基本 checklist
- 为什么不是所有 RISC-V 扩展都需要 GCC 支持
- RISC-V arch string 与 extension dependency 的关系
- 一个新 extension 进入 toolchain 前需要回答哪些问题
- RISC-V extension enablement 中 version、alias 和 dependency 的常见设计问题
- 如何为一个只影响汇编语法的扩展规划工具链支持

## GNU Binutils

- Binutils 支持一个 RISC-V 新扩展通常需要改哪些地方
- GAS testsuite 如何覆盖 RISC-V 新指令
- objdump 测试在 RISC-V extension 支持中的作用
- RISC-V opcode 表设计中的常见问题
- 从公开 patch 看 Binutils upstream review 关注点
- 如何检查一条新指令的 operand encoding 是否适合现有 opcode 表
- RISC-V disassembler 输出格式变化为什么需要测试
- GAS 对 arch string 和 extension dependency 的检查路径

## GCC RISC-V Backend

- GCC RISC-V backend 如何识别 target extension
- GCC builtin 和 intrinsic 的区别
- 如何从 RTL dump 定位 RISC-V backend 问题
- GCC testsuite 在 RISC-V 后端开发中的作用
- 为什么有些扩展适合 builtin，有些适合 auto codegen
- RISC-V backend 中 target hook、pattern 和 cost model 的分工
- 一个 backend codegen regression 的最小化分析流程
- 如何判断一个 ISA feature 是否应该暴露为 compiler option

## Toolchain CI

- RISC-V GNU Toolchain CI 应该覆盖哪些层次
- precommit CI 与 postcommit CI 的区别
- 工具链回归测试中的常见误区
- 如何分析一个 RISC-V 工具链 CI failure
- fuzzer result triage 的基本流程
- DejaGnu testsuite failure 的第一轮分类方法
- 如何区分环境问题、测试问题和真实 regression
- Toolchain CI 中 cross target、multilib 和 simulator 组合的取舍

## Open Source Upstreaming

- 如何向 GNU 工具链社区提交 RISC-V patch
- Reviewed-by、Acked-by 和 maintainer approval 的区别
- 开源社区中如何写清楚 patch motivation
- 技术 patch 之外，为什么沟通也很重要
- 从公开 mailing list 学习工具链社区协作
- 一个 RISC-V toolchain patch series 应该如何拆分
- 如何写一封便于 review 的 GCC / Binutils patch cover letter
- 公开 review 中如何回应 technical objection

## Specification Review from Toolchain Perspective

- 从 toolchain 角度 review RISC-V extension specification 应该看什么
- ISA extension 规范中的 encoding、mnemonic 和 operand 设计如何影响 Binutils
- 规范中的 feature dependency 如何影响 arch string 和 compiler options
- 为什么 specification 需要考虑 testsuite 和 diagnostics
- 从 compiler 角度看 instruction semantics 是否足够清晰
- 何时应该在 specification 阶段讨论 builtin、intrinsic 或 auto-vectorization
- RISC-V P extension 文档工作中可以抽象出的 toolchain review checklist
- 如何把 specification comment 写成可执行的 toolchain 建议

## Personal Technical Growth

- 如何把日常 toolchain debugging 转化成公开技术笔记
- 如何建立 GCC / Binutils patch review 的长期阅读习惯
- 写 RISC-V toolchain 文章时如何区分事实、经验和推断
- 从中文笔记过渡到 English summary 的方法
- 如何维护一个长期技术选题池
- 如何从公开 mailing list 中学习工程判断
- 如何复盘一个 RISC-V toolchain CI failure
- 如何把零散的 testsuite 经验整理成 checklist
