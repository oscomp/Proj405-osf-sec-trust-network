项目名称：基于国密算法的可信网络连接  
项目链接：https://strongswan.org/  
导师信息：霍文，15165077960，huowen@ieisystem.com  
难度：中  
分类：系统软件  

题目要求：  
- 实现基于 TPM2.0 或 TCM2.0 的可信网络连接功能；  
- 协议遵循 TNC（Trusted Network Connect）架构规范；  
- 支持国密算法（SM2/SM3/SM4）在身份认证、连接建立、远程度量等方面的应用；  
- 实现基于远程度量结果（PCR、Quote 等）的认证准入机制；  
- 最终能够实现一个支持国密算法的可信 VPN 连接系统；  

特征：  
- 开发语言：C/C++  
- 支持平台：TPM2.0、TCM2.0  
- 密码算法支持：SM2、SM3、SM4  
- 协议参考：TCG TNC 架构，国内可信连接架构（TCA）  
- 可扩展对接 strongSwan、libreswan 等开源 VPN 工具  
- 输出内容包括：身份认证、VPN通道建立、远程度量验证模块  

预期目标：  

**第一题：基础协议栈实现**  
- 实现基于 TPM2.0/TCM2.0 的远程身份认证协议栈；  
- 使用国密算法实现 VPN 连接身份鉴权（如基于 SM2 签名认证）；  
- 能通过 VPN 工具（如 strongSwan）发起可信连接；  

**第二题：基于可信认证的准入机制**  
- 实现远程测量报告生成与验证流程；  
- 度量内容支持 PCR 报告、TCG Quote 签名；  
- 根据度量结果动态判断是否允许设备连接网络资源；  

交付物清单：  
1. 核心代码：  
   - 实现可信连接协议模块  
   - 基于 TCM/TPM 国密算法支持的通信流程  
2. 文档：  
   - 使用说明文档（README）  
   - TPM2/TCM2 测试配置说明  
   - 测试流程与验证示例  

License：Apache-2.0

参考资料：  
1. TCG TNC 规范：  
   https://trustedcomputinggroup.org/wp-content/uploads/TCG-TNC-Architecture-for-Interoperability-Version-2.0-Revision-13-.pdf  
2. TNC 开源项目：  
   https://strongswan.org/  

备注：无  
