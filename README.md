# CMCC-SPTN-SBI-YANG
This project defines the YANG files used in SPTN (Software defined Packet Transport Network) southbound API ＆ definition of MPLS-TP OpenFlow protocol extensions for SPTN to accomplish the management and control of SPTN equipment.

1. sptn-ttp-2019.json is to give the definition of OpenFlow extensions for SPTN, which explains every filed needed in the extended OpenFlow table/group.

2. SPTN-SBI-YANG folder contains all the YANG files used in SPTN SBI. All the YANG files are defined based on OF-CONFIG V1.2. The folder includes:
- of-config-1.2.yang (basic OF-CONFIG specification)
- of-config-1.2-sptn-alarm.yang
- of-config-1.2-sptn-ces.yang (SPTN CES service module)
- of-config-1.2-sptn-clock.yang
- of-config-1.2-sptn-device.yang
- of-config-1.2-sptn-lag.yang (SPTN LAG protection module)
- of-config-1.2-sptn-link-oam.yang
- of-config-1.2-sptn-oam.yang
- of-config-1.2-sptn-port-ext.yang (SPTN port extensions module)
- of-config-1.2-sptn-qos.yang
- of-config-1.2-sptn-vpls.yang

This repository is created to support the China Mobile (CMCC) SPTN project. 

Any questions about this repository, please contact wangminxue@chinamobile.com, xuyunbin@caict.ac.cn or zhaoxing@caict.ac.cn.

2019年12月30日 提供最新版yang文件。
与之前相比：
1，增加了《of-config-1.2-sptn-event.yang》。
2，删除了《of-config-1.2-sptn-vpls.yang》。
3，《of-config-1.2-sptn-clock.yang》中的leaf-list system-clock-source-priority-list 增加 ordered-by user;
4，《of-config-1.2-sptn-lag.yang》将 lag 节点放入 "/of-config:capable-switch/of-config:resources"中，在 lag 节点中 加入 leaf openflow-port。
5，《of-config-1.2-sptn-link-oam.yang》将 loopback-status 拆分为 loopback-cmd 和 loopback-status。
6，《of-config-1.2-sptn-port-ext.yang》在 tdm 节点下增加 tdm-e1-status。用于控制器查询 TDM业务性能数据。
