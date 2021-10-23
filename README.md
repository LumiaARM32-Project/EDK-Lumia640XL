# EDK-Lumia640XLPkg
用于Lumia640XL的WIP定制ARM UEFI固件，基于rickliu的Lumia830Pkg：https://github.com/rickliu2000/Lumia930Pkg

## 支持状态
- EMMC MMU PMIC GPIO工作
- 部分ACPI(从WP中复制,目前未验证是否工作)

## 问题
- 在UEFI设置中，选择会一直向上，无法选择造项
- 无法启动Windows 

## 如何使用
- 编译:略
- 在EFIESP根下创建startup.nsh,在startup.nsh写exit并保存,然后引导 EDK2,会自动进入设置

## 感谢:
 - Rick Liu for creating Lumia930Pkg<br/>
 - Konrad Dybcio for creating Lumia535Pkg, a guide how to port edk2 to lumias and for helping me out when I was stuck<br/>
 - Imbushuo for creating BootShim<br/>
 - Heathcliff74 for creating WPInternals<br/>
