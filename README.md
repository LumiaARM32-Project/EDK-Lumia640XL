# EDK-Lumia640XLPkg
- 用于Lumia640XL的WIP定制ARM UEFI固件
- 基于rickliu的Lumia930Pkg：https://github.com/rickliu2000/Lumia930Pkg
- 原自Dominduchami的Lumia830Pkg：https://github.com/Dominduchami/Lumia830Pkg

## 支持状态
- EMMC MMU PMIC GPIO工作
- 部分ACPI(从WP中复制,目前未验证是否工作)

## 目前
- 部分ACPI(从WP中复制,目前未验证是否工作)
- 从UEFI.IMG的uefiplat.cfg中修复了DeviceMemoryMap(目前未验证是否工作)

## 问题
- 在UEFI设置中，选择会一直向上，无法选择选项
- 无法启动Windows (错误ConvertPages:Feiled to find range 10000000-10115FFF)

## 如何使用
- 编译:略
- 在EFIESP根下创建startup.nsh,在startup.nsh写exit并保存,然后引导 EDK2,会自动进入设置

## Linux
- 注:需要在UEFI shell用zImage启动(无ARMv7的grub支持),但目前未知启动参数,尚无法启动
- 需要一个设备树与内核。
- Lumia930:https://github.com/rickliu2000/linux_nokia_msm8974 (部分工作内核)
- Lumia830:https://github.com/Mainline4Lumia/linux/tree/msm8x26 (UART,EMMC工作内核)

## 感谢:
 - Rick Liu创作Lumia930Pkg<br/>
 - Konrad Dybcio用于创建Lumia535Pkg，指导如何将edk2移植到lumias<br/>
 - Imbushuo for creating BootShim<br/>
 - Heathcliff74 for creating WPInternals<br/>
 - Dominduchami<br/>
