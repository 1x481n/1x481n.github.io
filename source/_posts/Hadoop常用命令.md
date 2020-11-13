---
title: Hadoop常用命令
date: 2020-11-14 00:11:19
tags: 大数据,hadoop
---

1.查看 Job 信息：

```zsh
hadoop job -list
```
2.杀掉 Job：

```zsh
hadoop  job –kill  job_id
```

3.指定路径下查看历史日志汇总：

```zsh
hadoop job -history output-dir
```

4.作业的更多细节：

```zsh
hadoop job -history all output-dir
```

5.打印map和reduce完成百分比和所有计数器：

```zsh
hadoop job –status job_id
```

6.杀死任务。被杀死的任务不会不利于失败尝试：

```zsh
hadoop jab -kill-task
```

7.使任务失败。被失败的任务会对失败尝试不利：

```zsh
hadoop job  -fail-task
```

8、yarn资源管理器相关

```zsh
yarn application -list
```

如需杀死当前某个作业，使用kill application-id的命令如下：

```zsh
yarn application -kill application_1437456051228_1725
```