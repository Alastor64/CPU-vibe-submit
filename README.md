# RV32IM CPU Submission RTL

本仓库只保存由 `../vibe` 中 Chisel 源码生成的 Verilog/SystemVerilog。

生成文件是构建产物，禁止在此仓库手工修改 RTL。需要修改 CPU 行为时，应修改 Chisel
源码、重新生成并验证，然后以包含来源提交信息的独立提交更新本仓库。

提交 OJ 前必须保证：

- 顶层模块名为 `student_top`。
- `verilog/filelist.f` 只引用本仓库内实际存在的 RTL。
- 生成 RTL 已通过课程框架的 Verilator 编译、官方正确性测试和综合检查。
- 不包含本地绝对路径、缓存、波形或 AppImage。
