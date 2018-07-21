# Introduction

现实世界的数据通常都不干净。使用 Python 以及 Python 的库，你可以收集各种来源、各种格式的数据，评估数据的质量和整洁度，然后进行清洗。这个过程叫做数据整理。你可以在 Jupyter Notebook 中记录并展示数据整理的过程，然后使用 Python (及其库) 和/或 SQL 进行分析和可视化。

你将要整理 (以及分析和可视化) 的数据集是推特用户 [@dog_rates](https://twitter.com/dog_rates) 的档案, 推特昵称为 [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs)。WeRateDogs 是一个推特主，他以诙谐幽默的方式对人们的宠物狗评分。这些评分通常以 10 作为分母。但是分子则一般大于 10：11/10、12/10、13/10 等等。为什么会有这样的评分？因为 ["They're good dogs Brent."](http://knowyourmeme.com/memes/theyre-good-dogs-brent) WeRateDogs 拥有四百多万关注者，曾受到国际媒体的报道。

WeRateDogs [下载了他们的推特档案](https://support.twitter.com/articles/20170160)，并通过电子邮件发送给优达学城，专门为本项目使用。这个档案是基本的推特数据（推特 ID、时间戳、推特文本等），包含了截止到 2017 年 4 月 1 日的 5000 多条推特

# Dependencies

- 你需要在电脑上用 Jupyter Notebook 操作。请再次访问纳米学位课程中的 Anaconda 和 Jupyter Notebook 教程，作为安装指南。

- 需要安装下列软件包（即 Python 库）。你可以通过 conda 或 pip 安装这些库。请再次访问纳米学位课程中的 Anaconda 和 Jupyter Notebook 教程，作为文件包的安装指南。

  - pandas
  - numpy
  - requests
  - tweepy
  - json

# Project details

- 数据整理，其中包括：

  - 收集数据
  - 评估数据
  - 清洗数据

- 对清洗过的数据进行储存、分析和可视化
- 书面报告 1) 你的数据整理工作 和 2) 你的数据分析和可视化

# File overview

- sourse data

  - twitter_archive_enhanced.csv：给定的文件

- Intermediate data

  - image_predictions.tsv：以编程方式下载的文件
  - tweet_json.txt：通过 API 构建的文件
  - twitter_archive_master.csv：合并与清洗后的数据

- final data

  - wrangle_act.ipynb：用于收集、评估、清洗、分析和可视化数据的代码
  - wrangle_report.pdf：汇总数据整理步骤的文档：收集，评估和清洗
  - act_report.pdf：对最终数据进行观察与分析的文档
  - 其他附加文件（例如，用于存储干净数据的附加文件或数据库文件）
