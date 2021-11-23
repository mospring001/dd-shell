# 可在WebUI查看进度的一键DD脚本

## 脚本介绍

该脚本可在DD系统时为您提供一个WebUI以帮助您了解到目前的DD状态.

基于现有非常成熟的一键重装脚本修改, 只修改脚本内DD相关逻辑, 无任何学习成本.

暂只支持linux amd64.

## 特别感谢

Shell原作者: MoeClub

Shell二次修改: cxthhhhh

## 使用方法

基础用法同原始脚本, 高级用法可自行查看shell文件(部分功能可能未经过全面测试, 需要您自行承担后果)

## 演示图

TODO

## 风险说明

由于该脚本使用环境复杂, 故无法完全测试, 可能会导致您的服务器无法正常运行,数据丢失.

部分VPS商家明令禁止DD系统, 可能会导致您的服务器被终止.

DD时会占用较高资源, 可能导致您的服务器被暂停或终止.

作者无法知晓及监控用户行为, 也不承担对该脚本的任何责任(包括但不限于法律责任、数据损失责任)

## 技术相关说明

该脚本主要修改了原始的wget + gzip + dd步骤, 将其全部使用go实现, 同时加入了WebUI, WebUI与服务器之间通过ws进行沟通.

wget https://raw.githubusercontent.com/flyqie/dd-shell/master/Core_Install.sh && bash Core_Install.sh -d 10 -v 64 -a
