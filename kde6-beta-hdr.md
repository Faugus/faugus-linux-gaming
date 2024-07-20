Zamundaaa's Blog

https://zamundaaa.github.io/wayland/2023/12/18/update-on-hdr-and-colormanagement-in-plasma.html

Gamescope

https://github.com/ValveSoftware/gamescope

Vulkan HDR Layer

https://github.com/Zamundaaa/VK_hdr_layer

Vulkan HDR Layer on AUR

https://aur.archlinux.org/packages/vk-hdr-layer-kwin6-git

Zamundaaa's Steam launch command
```
ENABLE_HDR_WSI=1 gamescope --hdr-enabled --hdr-debug-force-output --steam -- env ENABLE_GAMESCOPE_WSI=1 DXVK_HDR=1 DISABLE_HDR_WSI=1 steam
```

Launch command used in the video
```
DXVK_HDR=1 ENABLE_HDR_WSI=1 gamescope -f -r 144 --hdr-enabled --hdr-debug-force-output -- env MANGOHUD=1 gamemoderun %command%
```
