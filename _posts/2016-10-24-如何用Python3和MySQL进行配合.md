---
layout: Blog Template for Bootstrap
title: 如何用Python3和MySQL进行配合
excerpt: 帮助大家绕开其中的一些坑
---
## 现状
Python3 已经成为了Python的趋势，但是因为一些兼容性问题，国内一些公司依然在使用Python2，比如Python3和MySQL无法完美的结合。

## 症状及解决办法
<table class = "table table-condensed">
<tr>
<th class="col-xs-4">症状</th>
<th class="col-xs-8">解决办法</th>
</tr>
<tr>
<td>哪个库适合Python3?</td>
<td>按照<a href="https://docs.djangoproject.com/el/1.10/ref/databases/#mysql-db-api-drivers">Django</a>的推荐，mysqlclient是不二的选择</td>
</tr>
<tr>
<td>在amazon linux上遇到mysql_config not found的错误</td>
<td>这个错误的原因是amazon linux上的mysql_config，不叫这个名字，而叫mysql_config55，所以可以用`ln /usr/bin/mysql_config55 /usr/bin/mysql_config`这样的命令手动链接一下</td>
</tr>
</table>
