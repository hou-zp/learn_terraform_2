## 使用说明

该样本间主要作用为创建ecs云服务器并将其挂载到slb负载均衡服务器上。

以下为该样本间会创建的资源:

- 创建名为tf_test_foo的vpc 专有网络。
- 在上述vpc下创建一台交换机。
- 创建默认安全组。
- 设置安全组规则，端口开放为 1/65535，白名单开放为0.0.0.0/0。
- 创建三台ecs云服务器。
- 创建slb负载均衡服务器，实例规格为slb.s2.small。并挂载上述创建ecs 服务器。

### 参考
关于阿里云更多terraform支持资源，请参考其官方文档 [Refer to details](https://github.com/aliyun/terraform-provider-alicloud)

