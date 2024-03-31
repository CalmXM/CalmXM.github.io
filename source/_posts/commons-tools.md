---
title: Windows常用配置 && 软件
abbrlink: 979000960
date: 2024-03-02 20:25:47
tags:
---

## 小鹤双拼一键配置

```reg
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\InputMethod\Settings\CHS]
"EnableExtraDomainType"=dword:00000001
"Enable Double Pinyin"=dword:00000001
"DoublePinyinScheme"=dword:0000000a
"UserDefinedDoublePinyinScheme0"="小鹤双拼*2*^*iuvdjhcwfg^xmlnpbksqszxkrltvyovt"
```

## 常用软件激活工具

| 软件 | 工具链接 |
|-----------------|-----------------|
| JetBrains全家桶 | [ja-netfilter](https://zhile.io/2021/11/29/ja-netfilter-javaagent-lib.html) |
| Microsoft office | [LKY_OfficeTools](https://github.com/OdysseusYuan/LKY_OfficeTools) |
| Windows激活工具 | [CMWTAT_Digital_Edition](https://github.com/TGSAN/CMWTAT_Digital_Edition) |

## Scoop

### 安装

```powershell
# 设置 PowerShell 执行策略
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
# 下载安装脚本
irm get.scoop.sh -outfile 'install.ps1'
# 执行安装, --ScoopDir 参数指定 Scoop 安装路径
.\install.ps1 -ScoopDir 'C:\Scoop'
```

### 配置

```powershell
# 设置代理
scoop config proxy 127.0.0.1:7890
# 取消代理
scoop config rm proxy
```

## 魔法

[青森云](https://y67w.cccc.gg/auth/register?code=AUCfGl)
