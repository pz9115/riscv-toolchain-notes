# RISC-V Toolchain Notes

记录 RISC-V GNU Toolchain、GCC、GNU Binutils、ISA extension enablement 和开源协作实践的技术笔记仓库。

仓库内容以中文为主，部分文章会逐步补充 English summary。

## 内容范围

- RISC-V ISA extension toolchain enablement
- GNU Binutils for RISC-V, including GAS and objdump
- GCC RISC-V backend
- GCC / Binutils testsuite
- RISC-V toolchain CI and regression analysis
- Open-source upstreaming notes
- Specification review from a toolchain perspective

## 仓库结构

```text
riscv-toolchain-notes/
  README.md
  LICENSE
  LICENSE-CODE
  topics.md
  drafts/
  published/
  talks/
  templates/
  examples/
  scripts/
```

- `topics.md`: 选题池。
- `drafts/`: 草稿和未完成的技术笔记。
- `published/`: 已发布或相对稳定的文章。
- `talks/`: 公开演讲, slides 和其他材料.
- `templates/`: 写作模板。
- `examples/`: 最小化的代码示例。
- `scripts/`: 写作、检查或仓库维护相关的辅助脚本。

## License

Articles, notes, diagrams, slides, and other non-code content are licensed under CC BY-NC-SA 4.0 unless otherwise noted.

Code snippets, examples, scripts, and tests are licensed under MIT License unless otherwise noted.

See [LICENSE](LICENSE) and [LICENSE-CODE](LICENSE-CODE) for details.

## Author

Jiawei Chen jiawei@iscas.ac.cn (ISCAS)

Focus: RISC-V GNU Toolchain / GCC / GNU Binutils / RISC-V ISA extension enablement
