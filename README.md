# JetsonTX2-display
How to setup two HDMI (x2) on Jetson, configurations, etc. Kernel 28.1


## What lines should be changed?

**Files**

-tegra186-quill-p3310-1000-c03-00-base.dtb

-tegra186-quill-p3310-1000-c03-00-dsi-hdmi-dp.dtb


```

nvdisplay@15200000{


status = "okay";

}

nvdisplay@15210000

{


status = "okay";

}

nvdisplay@15220000 {

status = "okay";

}

hdmi-display {

status = "okay";

}

sor {

status = "okay";

}

sor1 {

status = "okay";

}

```
## Files


You should replace 2 files on this directory during booting Jetson.

```
dtb  >>>>  /home/<directory-for-install-jetpack>/64_TX2/Linux_for_Tegra/kernel/dtb

```
