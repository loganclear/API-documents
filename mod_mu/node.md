# Node
最后修改：2021.4.29

路由 | 方式 | 参数 | 返回值 |描述
-----|------|-----|-------|----
`/nodes/{id}/info` | GET | node_id | node_group, node_class, node_speedlimit, traffic_rate, mu_only, sort, server, disconnect_time, type | 获取当前请求节点的节点设置

---
路由 | 方式 | 参数 | 描述
-----|------|-----|-------
`/nodes/{id}/info` | POST | node_id, load, uptime | 上报节点的负载和在线情况

---
路由 | 方式 | 参数 | 描述
-----|------|-----|-------
`/nodes` | POST | node_id, ip, user_id | 上报用户的当前在线IP
