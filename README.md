# Lumia830Pkg
WIP Custom ARM UEFI firmware for Lumia 830, based on Lumia830Pkg by rickliu : https://github.com/rickliu2000/Lumia930Pkg

# Current Status
Edk2 boots correctly, but it is not capable of loading windows (just use unlocked stock uefi for that). 
Linux boots with patches created by Bartosz Dudziak (https://patchwork.kernel.org/project/linux-arm-msm/list/?series=&submitter=193041&state=*&q=&archive=both&delegate=) and a simple dts (only UART and EMMC is enabled for now, display works via efiframebuffer).
A partially working kernel is available here : https://github.com/Dominduchami/linux

# Thanks to : <br/>
 - Rick Liu for creating Lumia930Pkg<br/>
 - Konrad Dybcio for creating Lumia535Pkg, a guide how to port edk2 to lumias and for helping me out when I was stuck<br/>
 - Imbushuo for creating BootShim<br/>
 - Heathcliff74 for creating WPInternals<br/>
