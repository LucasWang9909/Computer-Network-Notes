- 1.1 什么是互联网

  - 互联网是一个由**终端系统、通信链路、分组交换机、ISP** 组成的全球计算机网络
  - **协议** 是计算机网络的核心，控制着信息的传输和处理。
  - **TCP/IP 协议** 是互联网的基础，确保数据能正确传输到目的地。
  - 互联网不仅是物理网络，更是**应用的服务平台**，支持各种**分布式应用**。
  - **互联网标准（如 IETF、RFC）** 确保全球设备可以相互通信。

---

- 1.2 网络边缘
  - **终端系统通过接入网络连接到互联网**，主要包括 DSL、Cable、FTTH、5G 固定无线等。
  - **以太网和 WiFi 是家庭和企业常见的接入方式**，WiFi 更灵活，以太网更稳定。
  - **物理介质分为有线（双绞线、光纤）和无线（WiFi、蜂窝、卫星）**，不同技术适用于不同场景。

---

- 1.3 网络核心
  - **分组交换（Packet Switching）** 采用**存储-转发**方式，将数据拆分为**数据包**进行传输，提高带宽利用率，但可能出现**排队时延**和**丢包**。
  - **电路交换（Circuit Switching）** 需**预留端到端带宽**，确保稳定通信，但资源利用率低，现代通信逐步向**分组交换**发展。
  - **互联网是一个“网络的网络”**，由**分层 ISP（Tier-1, Tier-2, Tier-3）** 互联形成，采用 **IXP、Peering** 降低成本，提高效率。
  - **内容提供商（如 Google、Netflix）** 通过**CDN 和自建私有网络** 直连 ISP，减少对 Tier-1 依赖，优化内容传输。
  - **现代互联网是一个复杂的生态系统**，结合**ISP、IXP、CDN、Peering**，确保全球高效互联。

---

- 1.4 分组交换网中的时延、丢包和吞吐量
  - 计算机网络中的性能瓶颈主要体现为**延迟、丢包和吞吐量受限**。
  - **节点延迟**由处理、排队、传输和传播四部分构成，**排队延迟最不可预测**，易随流量强度剧烈变化；
  - **丢包**发生于队列溢出，**流量强度接近 1 时风险显著增加**；
  - **端到端延迟**可累加估算，工具如 _Traceroute_ 可实际观测路径和 RTT；
  - **吞吐量**由路径中最慢的链路决定，现代网络中通常由**接入链路或共享链路成为瓶颈**。
