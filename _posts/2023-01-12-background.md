---
title: 背景
author: 八百里
date: 2023-01-12
category: Jekyll
layout: post
---

目前市面是测试自动化工具框架层出不穷,api的有jmeter,postman,pytest，UI的有基于selenium封装的poium。种类繁多功能各异,基于我们目前现有的业务状况和大家的用例编写习惯,我们用pytest+playwight+allure做了一个工具,它可以录入api及UI测试用例。

## 实现功能
- 接口直接的数据依赖: 需要B接口使用A接口响应中的某个字段作为参数
- 动态多断言： 可（多个）动态提取实际预期结果与指定的预期结果进行比较断言操作
- 支持sql查询断言
- 支持UI测试用例编写,基于po模式
- 重写源码page及context方法，支持会话保持
- 测试完成自动生成allure测试报告