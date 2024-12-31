
# 什么是 lolMiner？详细教程与操作方法


## 什么是 lolMiner？

lolMiner 是一款专为 AMD 显卡设计的挖矿软件，同时也支持部分 Nvidia 显卡。然而，Nvidia 显卡在 lolMiner 上的运行速度和稳定性可能较差，官方开发者对此也有所提示。作为一款支持 Equihash 和 Cuckatoo 算法的挖矿工具，它以较高的更新频率和适配性，深受用户喜爱。

- **开发者费用**：1%（相当于每天运行 14 分钟用于开发者）。
- **适配显卡**：优化支持 AMD 显卡，部分 Nvidia 显卡兼容性较差。

---

## lolMiner 支持的挖矿算法

lolMiner 支持多种算法，可用于挖掘多种数字货币。以下为推荐的 GPU 内存需求和支持的算法：

| **算法**                | **支持币种**                     | **推荐 GPU 内存**  |
|-------------------------|----------------------------------|-------------------|
| Equihash 96.5          | MinexCoin                       | 1.3 GB           |
| Equihash 144.5         | Bitcoin Gold, BitcoinZ, SnowGem | 1.8 GB           |
| Equihash 125.4         | ZelCash                         | 2.9 GB           |
| Equihash 150.5         | Beam                            | 2.7 GB           |
| Equihash 192.7         | Zero, Genesis Network           | 3 GB             |
| Equihash 210.9         | Aion                            | 1 GB             |
| Cuckarood 29           | Grin                            | 3.8/5.5 GB       |
| Cuckatoo 31            | Grin                            | 3.8/7.8 GB       |

### 最新更新
- 移除 Beam hardfork 后不再适用的 BeamHash I 算法。
- 优化 Nvidia 显卡在 Beam 算法中的性能（推荐使用 Gminer 挖掘 Beam）。

---

[欧易迎新限时福利，领取最高 100 USDT 奖励](https://bit.ly/OKXe)

使用限时注册福利内部邀请码：**8265080** 成功完成账号注册后领取！

---
## lolMiner 的 GPU 哈希率测试

以下为不同显卡在 lolMiner 上的测试哈希率结果：

### Nvidia 显卡性能
- **Nvidia GTX 1060**：15 sol/s  
- **Nvidia GTX 1070**：23–25 sol/s  
- **Nvidia GTX 1070 ti**：26 sol/s  
- **Nvidia GTX 1080**：21–24 sol/s  
- **Nvidia GTX 1080 ti**：40 sol/s  

### AMD 显卡性能
- **AMD Radeon RX 480 4 GB**：15–16 sol/s  
- **AMD Radeon RX 570**：14.5–15 sol/s  
- **AMD Radeon RX 580 8 GB**：26 sol/s  

**提示**：如果目标是最大化收益，建议使用 AMD 显卡挖掘以太坊或以太坊经典。通过 [2CryptoCalc](https://2cryptocalc.com/) 计算器，可以实时选择最具盈利潜力的加密货币。

---

## 如何下载 lolMiner

lolMiner 可从以下两个主要来源下载：
1. **[BitcoinTalk 官方页面](https://bitcointalk.org/index.php?topic=4724735.0)**  
2. **[2Miners 快速入门档案](https://drive.google.com/file/d/11R0L-QgOHnzZ5JfxidH2KPYj1PFEeqDY/view?usp=sharing)**（存档密码：2miners）

---

## 如何设置 lolMiner

以下是基于 ZelCash 挖矿的配置示例，使用的是 [2Miners](https://2miners.com/) 挖矿池。

### 配置步骤
1. 创建一个 `.bat` 文件，写入以下命令：
   ```plaintext
   setx GPU_FORCE_64BIT_PTR 1
   setx GPU_MAX_HEAP_SIZE 100
   setx GPU_USE_SYNC_OBJECTS 1
   setx GPU_MAX_ALLOC_PERCENT 100
   setx GPU_SINGLE_ALLOC_PERCENT 100
   ```

2. 添加以下代码运行 lolMiner：
   ```plaintext
   lolMiner.exe --coin ZEL --pool zel.2miners.com --port 9090 --user YOUR_ADDRESS.RIG_ID --pass x
   ```

### 参数说明
- **YOUR_ADDRESS**：填写您的真实钱包地址（如：`t1JKRwXGfKTGfPV1z48rvoLyabk31z3xwHa`）。
- **RIG_ID**：矿机的名称，推荐设置一个唯一名称，支持32个字符，包括字母、数字及符号 `-` 和 `_`。

### 启动后效果
运行 `.bat` 文件后，界面将显示挖矿状态信息，类似以下截图：

![lolMiner 挖矿界面](https://www.yundongfang.com/wp-content/uploads/2021/10/image6.jpg)

---

## lolMiner 总结

lolMiner 是一款高效的 AMD 挖矿工具，适用于挖掘 Equihash 和 Cuckatoo 算法的币种。尽管对 Nvidia 显卡的支持稍显不足，但其强大的 AMD 性能补足了这一点。此外，lolMiner 的持续更新也确保了软件的竞争力。

[欧易迎新限时福利，立即领取](https://bit.ly/OKXe)  
使用邀请码 **8265080**，注册即可领取最高 100 USDT 的奖励！

开始挖矿吧，祝您拥有愉快的收益体验！
