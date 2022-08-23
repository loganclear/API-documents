# User
最后修改：2021.4.29

路由 | 方式 | 参数 | 返回值 |描述
-----|------|-----|-------|----
`/users` | GET | node_id | 见下表 | 获取当前请求节点（根据 node_id 参数判断）可连接的用户

节点类型 | 下发的数据
--------|--------
SS/SSR | method, obfs, obfs_param, protocol, protocol_param, node_speedlimit,is_multi_user, u, d, transfer_enable, id, port, passwd, node_connector, alive_ip
V2Ray  | node_speedlimit, u, d, transfer_enable, id, node_connector, uuid, alive_ip
Trojan | node_speedlimit, u, d, transfer_enable, id, node_connector, uuid, alive_ip

---
路由 | 方式 | 参数 | 描述
-----|------|-----|-------
`/users/traffic` | POST | node_id, u, d, user_id | 上报用户的流量使用情况

---
路由 | 方式 | 参数 | 描述
-----|------|-----|-------
`/users/aliveip` | POST | node_id, ip, user_id | 上报用户的当前在线IP

---
路由 | 方式 | 参数 | 描述
-----|------|-----|-------
`/users/detectlog` | POST | node_id, list_id, user_id | 上报用户碰撞的审计规则id
