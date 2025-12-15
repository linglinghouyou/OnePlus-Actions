# ⭐⭐⭐ Star This Project ⭐⭐⭐

如果您觉得这个项目对您有帮助，请给我一个 star / 进行赞助！您的支持是我持续改进的动力，如果遇到问题欢迎提交issue！也随时欢迎pr！

<img width="250" height="250" alt="image" src="https://github.com/user-attachments/assets/55acad97-8fe6-4de7-b9ce-90da9552a212" />

## OnePlus 开源地址

[![OnePlus Repository](https://img.shields.io/badge/OnePlus-Repository-red)](https://github.com/Xiaomichael/kernel_manifest)

## 设备支持

支持欧加真内核版本 `5.10-6.6` 的设备，只要跑出来内核版本号一样就可以用

## 使用指南

### ① 分支选择

1. 点击 `Branches` 切换处理器分支
2. 选择适合您设备的配置[如下图，如果找不到代号名称去网上搜搜]

<img width="219" height="488" alt="image" src="https://github.com/user-attachments/assets/a62811aa-357d-4645-830c-002e7a7f6e03" />

### ② 配置文件说明

以**一加12**为例：
- `_b` 后缀：ColorOS 16
- `_v` 后缀：ColorOS 15
- `_u` 后缀：ColorOS 14
- `_t` 后缀：ColorOS 13

<img width="1122" height="257" alt="image" src="https://github.com/user-attachments/assets/24631b01-ec9d-4f77-a764-476cfe522537" />

### ③ 配置开关建议

- **SUSFS选项**：SUSFS在 最新版 `KernelSU` 与 `SukiSU Ultra` 上已经改为可选，看你的需求进行开关 
- **KPM选项**：建议禁用以减少电量消耗，挂🐕去④
- **lz4kd**：
  - 6.1系列内核：建议关闭该选项以获得更好的 `lz4 + zstd` 压缩方式
  - 6.6系内核：建议关闭该选项以获得更好的 `lz4` 压缩方式
  - 其他内核版本：建议保持开启
- **BBR算法**：对手机日用无太大意义甚至可能负优化，推荐关闭
- **BBG基带守护**: 当然推荐开启，看名字就知道是干啥的
- **⚠️代理优化⚠️**: 骁龙芯片可以开，联发科芯片 `千万不要开` ，否则出现恶性Bug！
