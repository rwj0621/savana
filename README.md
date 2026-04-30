# [savana](https://github.com/cortes-ciriano-lab/savana)
## 一、安装工具
### 1. 创建环境
        conda create -n savana -y
### 2. 激活环境
        conda activate savana
### 3.安装[savana](https://github.com/cortes-ciriano-lab/savana#installation)
* 根据官方指南，直接用conda安装

        conda install savana
### 4.验证安装
* 成功显示版本即为安装成功（1.3.7）
        savana --version
## 二、运行savana
需要定义[config](https://github.com/rwj0621/savana/blob/main/contigs.chr.hg38.txt)列表，不然运行时候会报错

        savana --outdir /data/renweijie/Softwares/SV_tools/savana/HCC1395_HIFI \
        --tumour /data/renweijie/data/HCC1395/HCC1395_HiFi/tumor/HCC1395.GRCh38.bam \
        --normal /data/renweijie/data/HCC1395/HCC1395_HiFi/normal/HCC1395-BL.GRCh38.bam \
        --ref /data/renweijie/data/GRCh38/GRCh38.d1.vd1.fa \
        --length 50 \
        --pb \
        --sample HCC1395 \
        --contigs /data/renweijie/Softwares/SV_tools/savana/contigs.chr.hg38.txt \
        --threads 8
