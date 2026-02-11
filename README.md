# Vmware安装win11提示这台电脑无法运行Windows 11解决方法
问题如下：<br>
![iamge](https://github.com/IThuanghao/Vmware-win11-Windows-11--already-exists-in-this-account/blob/main/Vmare_win11_image/1.png)<br>

碰到上面的提示问题怎么办，首先关闭这个虚拟机，之后去设置一下虚拟机。

关机后检查一下你创建的虚拟机硬件是什么配置，windows11 最低要求是2核心CPU，4GB内存，64GB 硬盘空间，配置高于最低要求那么可以继续下一步<br>
![image](https://github.com/IThuanghao/Vmware-win11-Windows-11--already-exists-in-this-account/blob/main/Vmare_win11_image/2.png)<br>

打开虚拟机设置：进入选项，找到高级-->固件类型下面选择为UEFI   <br>
![image](https://github.com/IThuanghao/Vmware-win11-Windows-11--already-exists-in-this-account/blob/main/Vmare_win11_image/3.png)   <br>

接下来设置访问控制，默认这一项是未加密的，在vmware workstation Pro17目前版本来看的话是必须要设置的，否则在下一步添加可信平台模块是不能通过的。

![image](https://github.com/IThuanghao/Vmware-win11-Windows-11--already-exists-in-this-account/blob/main/Vmare_win11_image/4.png)   <br>

设置完密码就会出现下图，证明设置成功了。  <br>
![iamge](https://github.com/IThuanghao/Vmware-win11-Windows-11--already-exists-in-this-account/blob/main/Vmare_win11_image/5.png)  <br>

接下来在到硬件选项卡下点击添加，弹出一个添加硬件向导的窗口，在这个窗口中选择“可信平台模块”点击下一步就可以了。这一步正常是需要设置密码的，所以在上一步要求必须设置密码，否则无法添加。  <br>
![image]([https://github.com/IThuanghao/Vmware-win11-Windows-11--already-exists-in-this-account/blob/main/Vmare_win11_image/6.png0](https://github.com/IThuanghao/Vmware-win11-Windows-11--already-exists-in-this-account/blob/main/Vmare_win11_image/6.png))  <br>
如果你测试很多次发现必须用BIOS才能正确启动系统，可是添加可行平台模块又需要使用uefi启动  <br>
那么你就遇到了跟我一样的问题了  <br>
解决办法就是启动后一直按enter键<br>
在出现超时页面前，快速按回车<br>
