# 简介

-------------------------------------------
马上过年了，又到了发红包的时间，抢红包又蠢蠢欲动了，所以利用Android无障碍服务实现了一个微信自用抢红包辅助，好快速抢家里长辈发的红包哈哈。


# 使用
下载[红包辅助](https://github.com/gemgao/redenvelopes/tree/master/app/release "红包辅助")，打开红包辅助，打开无障碍，通知权限，然后就可以了

# 更新记录
1.0.8   **适配微信8.0.0,** ps:微信8.0的改动非常大，个人感觉越来越qq化了，毕竟年轻人才是未来。8.0版本小米10默认版本延迟增加到了150毫秒才可以。别的手机请自行调整。

1.0.7  适配微信7.0.19，ps:微信的检测机制也在完善，19版本在点击红包item的时候也要延迟，不然取不到节点，并且测试小米10延迟需要100毫秒了。

**猜想**：以后的微信版本会不会获取每个节点都要延迟才能获取呢？

1.0.6  增加自己在界面设置延迟时间，不需要代码改

1.0.5 适配微信7.0.18.

由于微信做了限制，在开红包的弹窗获取不到'开'的id节点，并且第一次获取不到，以后也获取不到，经过测试，发现必须延迟一定的时间，才能获取到，小米10是延时80毫秒可以，

`  val delayTime = 80L//小米10测试数据
 `

别的手机只要调整延迟时间就都可以。ps：这个不是最好的解决方法，，谁有好方法可以提供一下。

1.0.4 适配微信7.0.13

1.0.3 适配微信7.0.12  ps：由于微信7.0.12改版较大，只能保证微信7.0.12版本正常，低版本微信请用1.0.2

1.0.2 适配微信7.0.10

1.0.1 适配微信7.0.9

1.0.0 初始化项目，适配了微信7.0.3,7.0.4,7.0.5,7.0.8
# 适配

手机版本：因为Android手机太多，目前我只有自用的华为v9，oppoR9测试过，别的手机理论上都可以，如果有不行的，请及时提isu

# 感谢
本项目依据 https://github.com/xbdcc/GrabRedEnvelope 改写而来。做了新的适配。
