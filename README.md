# zzuthesis

郑州大学 ~~本科毕业设计(论文)和~~ 研究生专业学位论文(含 硕士 ~~和博士~~) LaTeX 模版。 ~~本科毕业设计（论文）和研究生学位论文（含硕士和博士） 分别根据《郑州大学材料科学与工程学院本科毕业设计（论文）基本规范》和《郑州大学学位论文写作规范格式》的规范要求制定。~~ 硕士研究生专业学位论文根据《郑州大学学位论文写作规范格式》的规范要求制定。该模板主要完成于 2012 年上半年，在上传至 Github 前进行了部分调整，以保证正常编译运行。2023 年 10 月进行了部分修改。

## 1. 字体配置

采用 ctex 宏包中的字体配置。
**需要 Windows 字体**

## 2. 模板编译

该模板分别在 ~~Windows 和~~ Linux 平台安装的 TeXLive 2022 下测试通过。

### 2.1 模板文件的生成

  `latexmk -xelatex main`

### 2.2 A3 封面文件的生成

  `xelatex spine`
  
  `xelatex a3cover`

### 2.3 自动运行脚本(Makefile)

* `make all`       等于 `make thesis && make a3cover`(默认选项)；
* `make thesis`    生成论文 main.pdf；
* `make a3cover`   生成封面 a3cover.pdf；
* `make clean`     清理中间文件；
