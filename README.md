# Multi-size THP for Anonymous Memory

[English](#english) | [中文](#中文)

---

## English

### Overview
This repository contains a comprehensive analysis and integration guide for the **Multi-size Transparent Huge Pages (mTHP) for Anonymous Memory** feature introduced in Linux kernel 6.8, with a focus on backporting to OpenEuler 6.6.

### What is Multi-size THP?
Multi-size THP is a runtime opt-in feature that improves performance by allocating larger chunks of memory during anonymous page faults. Unlike traditional THP which only supports fixed 2MB pages, mTHP supports multiple sizes (64KB, 128KB, 256KB, 512KB, 1MB, 2MB) providing more flexibility.

### Key Features
- 🎯 Multiple THP sizes support
- ⚙️ Runtime configuration via sysfs
- 📊 Per-size allocation statistics
- 🔧 ARM64 architecture optimizations
- 🚀 Improved page fault performance
- 🌐 NUMA balancing support

### Repository Contents

**Core Documentation:**
- **README_CN.md** - Comprehensive Chinese documentation
- **INDEX.md** - Complete file index and reading guide
- **PATCH_SUMMARY.md** - Patch summary with commit list
- **CODE_COMPARISON.md** - Detailed code comparison analysis
- **Multi-size_THP_Integration_Report.xlsx** - Comprehensive Excel report

**Technical Files:**
- **multi-size-thp-unified.patch** - Unified patch file
- **mthp_commits_info.json** - Structured commit information
- **scripts/** - Helper scripts for document generation

### Quick Start
1. Read `README_CN.md` for complete overview
2. Check `INDEX.md` for document navigation
3. Review `Multi-size_THP_Integration_Report.xlsx` for detailed analysis

### Statistics
- **Commits**: ~10 major commits
- **Files Changed**: ~12-15 files
- **Code Added**: ~2,600 lines
- **Code Removed**: ~300 lines
- **Net Change**: ~2,300 lines

### Main Contributor
- Ryan Roberts (ARM)

---

## 中文

### 项目概述
本仓库包含了Linux 6.8内核中引入的**多尺寸透明大页(mTHP)匿名内存**特性的完整分析和OpenEuler 6.6集成指南。

### 什么是Multi-size THP?
多尺寸THP是一项运行时可选特性，通过在匿名页错误期间分配更大的内存块来提高性能。与传统的仅支持固定2MB页面的THP不同，mTHP支持多种大小(64KB、128KB、256KB、512KB、1MB、2MB)，提供更大的灵活性。

### 主要特点
- 🎯 支持多种THP大小
- ⚙️ 通过sysfs运行时配置
- 📊 每种大小的分配统计
- 🔧 ARM64架构优化
- 🚀 改进页错误性能
- 🌐 NUMA平衡支持

### 仓库内容

**核心文档:**
- **README_CN.md** - 完整的中文文档
- **INDEX.md** - 完整的文件索引和阅读指南
- **PATCH_SUMMARY.md** - 包含提交列表的补丁摘要
- **CODE_COMPARISON.md** - 详细的代码比对分析
- **Multi-size_THP_Integration_Report.xlsx** - 综合Excel报告

**技术文件:**
- **multi-size-thp-unified.patch** - 统一补丁文件
- **mthp_commits_info.json** - 结构化提交信息
- **scripts/** - 文档生成辅助脚本

### 快速开始
1. 阅读 `README_CN.md` 获取完整概述
2. 查看 `INDEX.md` 了解文档导航
3. 查阅 `Multi-size_THP_Integration_Report.xlsx` 进行详细分析

### 统计数据
- **提交数**: 约10个主要提交
- **修改文件**: 约12-15个文件
- **新增代码**: 约2,600行
- **删除代码**: 约300行
- **净变更**: 约2,300行

### 主要贡献者
- Ryan Roberts (ARM)

### 文档语言
所有核心文档均提供详细的中文说明，便于国内开发者理解和使用。

---

**License**: Documentation under CC BY 4.0, Kernel code under GPL-2.0
**Last Updated**: 2024-12-17