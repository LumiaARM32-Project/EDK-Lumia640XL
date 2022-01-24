# EDK-Lumia640XLPkg
- 用于Lumia640XL的WIP定制ARM UEFI固件
- 基于rickliu的Lumia930Pkg:https://github.com/rickliu2000/Lumia930Pkg
- 原自Dominduchami的Lumia830Pkg:https//github.com/Dominduchami/Lumia830Pkg

## 
- 目前Linux的网络不能支持，也许将会停止进行

## 进行
- 无

## EDK-UEFI支持状态
- EMMC MMU PMIC GPIO工作
- 部分ACPI（从WP中复制，目前未验证是否工作）
- 已有GRUB支持
- 可以启动Linux-arm
- 可以引导bootarm.efi(windows启动管理器)

## Linux中支持状态
- EMMC 触屏--工作

##  Linux
- 注：需要在UEFI shell用zImage或启动GRUB，目前已经可以启动
- 需要一个设备树（dtb）与内核。
- Lumia930：https://github.com/rickliu2000/linux_nokia_msm8974 (只适用于930，部分工作)
- Lumia830：https://github.com/Mainline4Lumia/linux/tree/msm8x26 (UART，EMMC，触屏工作内核)

## 问题
- 在UEFI设置中，选择会一直向上，无法选择选项
- 可以引导bootarm.efi(在uefi shell),但加载Windows没有微标，一直黑屏（我认为启动Windows没有意义，除非windows lot）

## 如何使用
- 编译:略
- 在EFIESP根下创建startup.nsh，在startup.nsh写exit并保存，然后引导 EDK2，会自动进入设置

## 感谢：
 - Rick Liu创作Lumia930Pkg<br/>
 - Konrad Dybcio用于创建Lumia535Pkg，指导如何将edk2移植到lumias<br/>
 - 用于创建 BootShim<br/> 的 Imbushuo
 - Heathcliff74 用于创建 WPInternals<br/>
 - 多明杜哈米<br/>
