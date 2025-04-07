<!--
 * @Author: wzdnzd
 * @Date: 2022-03-06 14:51:29
 * @Description: 
 * Copyright (c) 2022 by wzdnzd, All Rights Reserved.
-->

## 功能
打造免费代理池，爬一切可爬节点
> 拥有灵活的插件系统，如果目标网站特殊，现有功能未能覆盖，可针对性地通过插件实现

> 欢迎 Star 及 PR。对于质量较高且普适的爬取目标，亦可在 Issues 中列出，将在评估后选择性添加

## 使用方法
> 可前往 [Issue #91](https://github.com/wzdnzd/aggregator/issues/91) 食用**共享订阅**，量大质优。**请勿浪费**
 
略，自行探索。我才不会告诉你入口是 `collect.py` 和 `process.py`。**强烈建议使用后者，前者只是个小玩具**，配置参考 `subscribe/config/config.default.json`

## 获取方法

1.谷歌colab
https://colab.research.google.com

2.在新建的笔记本中，运行以下命令以克隆项目仓库：​

    !git clone https://github.com/wzdnzd/aggregator.git

3.安装依赖项(有可能不用)：

  进入克隆的项目目录：​

    %cd aggregator

  安装项目所需的 Python 依赖项：​

    !pip install -r requirements.txt

4.运行项目：

  在 Colab 中，使用以下命令运行 process.py 脚本：

    !python -u subscribe/collect.py -s
  或(推荐下面)
  
    !python -u subscribe/process.py -s

5.查看节点文件：

    !cat /content/aggregator/data/v2ray.txt

6.下载节点文件

    from google.colab import files
    files.download('/content/aggregator/data/v2ray.txt')


## 免责申明
+ 本项目仅用作学习爬虫技术，请勿滥用，不要通过此工具做任何违法乱纪或有损国家利益之事
+ 禁止使用该项目进行任何盈利活动，对一切非法使用所产生的后果，本人概不负责
