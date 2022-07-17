# MUX VLAN(MultiComplex VLAN)



###### MUX VLAN技术术语：

| MUX VLAN              | VLAN类型                                                     | 所属端口                                                  | 通信规则                 |
| --------------------- | ------------------------------------------------------------ | --------------------------------------------------------- | ------------------------ |
| Principal VLAN 主VLAN |                                                              | Principal Port 主端口                                     | 可以和所有VLAN通信       |
| Subordinate 从VLAN    | Group VLAN（互通型<font color = red>VLAN</font>) 和 Separate VLAN （隔离型从VLAN) | Group Port（互通型从端口），Separate Port（隔离型从端口） | 只能和Principal VLAN通信 |

###### Super VLAN(聚合VLAN)

可以实现在相同网段但不同VLAN之间的用户通信。

> 目的：节约IP地址的浪费。

Super-VLAN只建立三层的VLANIF接口（虚拟）

Sub-VLAN只建立物理接口，不建立三层接口，隔离广播域。

> 通过建立Super-VLAN和Sub-VLAN间的映射关系，吧三层虚拟接口和物理接口结合起来，从而在实现普通VLAN功能的同时节省IP地址的目的。

![image-20220717004457448](C:\Users\yangc\AppData\Roaming\Typora\typora-user-images\image-20220717004457448.png)

所有Sub-VLAN共用同一个网段。

不同Sub-VLAN下的主机默认不能相互通信，要通信

需要在Super-VLAN的接口上开启代理ARP。