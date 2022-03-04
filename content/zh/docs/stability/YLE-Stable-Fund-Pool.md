---
title: "YLE稳定基金池"
description: "One page summary of how to start a new Doks project."
lead: "One page summary of how to start a new Doks project."
date: 2020-11-16T13:59:39+01:00
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
menu:
  docs:
    parent: "stability"
weight: 105
toc: true
---

![img](https://2921122931-files.gitbook.io/~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-MZVvE5_ih-8CBheubxy%2F-Mij7dMnpLlb_ZDKtGcr%2F-Mij86TMPVm_7AtBLmtk%2F%E5%B9%BB%E7%81%AF%E7%89%8713.JPG?alt=media&token=02942e39-6522-4074-a333-e1380494e509)

## **稳定基金池自动交易机制**

YLE内设立了稳定基金池，其作用是使用稳定基金池内的资金，通过自动化SWAP交易平衡和稳定YL的市场交易价格。

当YL的价格在基准价格区间（±0.02）内，稳定基金池不作为。

当YL价格发生偏离时，稳定基金池开始启动，先动用基金池内被交易TOKEN 0.1%的资金，优先成交偏离价订单。成交完，如果稳定基金池相应的资金量不足以完全成交，不足的部分再从农场资金池的Swap交易中获得。交易价格每偏离加大0.01，基金池动用的总资金在上一次的资金数额上翻倍。

> 比如，当YL价格涨到1.02USDT时，稳定基金池按照当时订单价格，优先出售池中0.1%的YL。价格涨到1.03U时，优先出售池中0.2%的YL。1.04U时，优先出售0.4%YL。价格每涨0.1%，稳定基金优先出售比例翻倍。

## **稳定基金池的资金来源**

1. YLS稳定共享积分拍卖收入的80% 
2. YLE生态内交易手续费的80% 
3. 无常滑点交易手续费的80% 
4. 蓄水池按用户耕种收益的4%划拨 
5. 本田调整质押资金手续费的80%
