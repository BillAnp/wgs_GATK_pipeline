[TOC]



# 前言

本文是基于GATK4，整理出的shell流程为基础的WGS系列数据分析的主体流程。

# 单样本模式

## 说明
集合到一个shell脚本中，文件名为wgs_single.sh，这个流程假设只有一对Illumina的PE测序数据文件。含有6个参数
* read1 的 path
* read2 的 path
* Read group ID
* 测序文库编号
* 样本编号
* output path

## 用法
``` shell
sh wgs_single.sh read1.fq.gz read2.fq.gz Test_RG Test_lib Test_sample Test_outdir
```

## shell脚本代码

