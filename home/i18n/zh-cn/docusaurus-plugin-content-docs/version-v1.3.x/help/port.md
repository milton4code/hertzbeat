---
id: port  
title: 监控：端口可用性      
sidebar_label: 端口可用性    
keywords: [开源监控系统, 开源网络监控, 端口可用性监控]
---

> 判断对端服务暴露端口是否可用，进而判断对端服务是否可用，采集响应时间等指标进行监测

### 配置参数

| 参数名称      | 参数帮助描述 |
| ----------- | ----------- |
| 监控Host     | 被监控的对端IPV4，IPV6或域名。注意⚠️不带协议头(eg: https://, http://)。 |
| 监控名称     | 标识此监控的名称，名称需要保证唯一性。  |
| 端口        | 网站对外提供的端口，http一般默认为80，https一般默认为443。  |
| 连接超时时间 | 端口连接的等待超时时间，单位毫秒，默认3000毫秒。  |
| 采集间隔    | 监控周期性采集数据间隔时间，单位秒，可设置的最小间隔为30秒  |
| 是否探测    | 新增监控前是否先探测检查监控可用性，探测成功才会继续新增修改操作  |
| 描述备注    | 更多标识和描述此监控的备注信息，用户可以在这里备注信息  |

### 采集指标

#### 指标集合：summary

| 指标名称      | 指标单位 | 指标帮助描述 |
| ----------- | ----------- | ----------- |
| responseTime   | ms毫秒 | 网站响应时间 |

