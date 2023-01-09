# Linux桌面环境&窗口管理器介绍（介绍的都是我推荐的） by ZhaoymOvO
> 这篇文章在[署名-非商业性使用-相同方式共享 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/)协议下提供，转载请遵守[署名-非商业性使用-相同方式共享 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/)协议

---
## 桌面环境御三家
> 桌面环境提供了完整的GUI支持以及更多的自定义选项，或许是你使用的首选。

### KDE Plasma
KDE Plasma是御三家中最早出现的桌面环境。  
Plasma采用了Qt框架，并且最近加入了Wayland显示服务支持。  
Plasma是御三家中自定义最简单的、插件最多的桌面环境，同时原生观感就很棒，也可以原生实现很炫酷的动画效果。  
得益与插件，Plasma可以配置成类似Windows的外观（以及操作逻辑），也可以是Mac OS，或者任何你喜欢的样式。  
Plasma是御三家当中优化最好的，它是一个重量级桌面环境，但是资源占用（除磁盘占用外）都快要和Xfce4（御三家，轻量级桌面环境）相当了。

### GNOME
GNOME因RedHat而生（RedHat不希望被Qt的使用条款限制他的商业行为），是御三家中第二位出生的。  
GNOME采用了GTK框架（不是GNOME tool kit是GIMP tool kit），并且是御三家中最早支持Wayland显示服务的，也是对Wayland显示服务支持最完善的（毕竟Wayland也是RedHat整的）。  
GNOME是御三家当中生态统一做的最好的桌面环境，这也使御三家内GNOME可以最方便的配置代理。   
不过这也导致了想要**自定义GNOME只能依靠插件**，但是GNOME插件在更新GNOME版本后一般都不能继续使用。  
GNOME的操作逻辑在御三家乃至整个Linux桌面环境中是最适合触屏设备的。硕大的按钮、Android一般的状态栏，对触控设备很有好。  
GNOME是一个重量级桌面环境，也是御三家当中优化最差的。

### Xfce4
Xfce是御三家中存在感最弱，也是最小的一位，稳定（更新慢）。  
Xfce4中的4指的是Xfce4.x版本。  
Xfce4使用GTK框架，**不支持**Wayland显示服务。  
Xfce4的自定义程度很高，默认的主题（Graybird）是御三家中唯一仍在使用的**纯拟物**主题（Breeze和Adwaita是半拟物，前者偏扁平，后者偏拟物），但是插件数量**很少**，且基本都是官方插件。  
Xfce4是御三家中最轻量的桌面环境，占用最低，不过应该是牺牲丰富的功能和动画效果换来的，实际优化应该没有KDE Plasma好。  
虽说Xfce4牺牲了很多的功能和效果来换取性能，但是Xfce4用于日常使用是完全没有问题的。

---
## 窗口管理器双雄争霸
> 窗口管理器提供基本的多窗口管理服务，如果性能真的捉急，这可能是你的备选项，或者你只是希望更高的硬件效率。自定义空间极大（难度也是）。

### OpenBox
OpenBox是一个使用较为广泛的**堆叠式**窗口管理器不支持Wayland显示服务。  
OpenBox是LXDE和LXQt默认使用的窗口管理器。  
OpenBox不包含Panel、Dock之类的东西，也没有桌面图标、壁纸支持，切换最小化的窗口请使用Alt+Tab，桌面右键可以呼出应用程序菜单。  
### i3wm/sway
i3wm（接下来统称i3）是一个**平铺式**窗口管理器，不支持Wayland显示服务。  
i3包含一个Dock，上面显示了基本信息。 
i3所有的窗口管理操作都通过键盘实现。  
sway可以看成是i3的Wayland实现，只支持Wayland。  

---
## 其他桌面环境
> 我只会写我建议的而不是市面上常见的，请见谅。

### LXDE/LXQt
二者出自同一团队之手，LXDE可以看作是LXQt的前代，LXDE现已停止维护。  
LXDE使用了GTK框架，LXQt使用了Qt框架，二者默认使用OpenBox窗口管理器，可以自定义修改。  
自定义程度不高，默认界面十分的拟物，不过二者的主要卖点是轻量，更甚于Xfce4。  
### MATE
MATE桌面环境是GNOME 2的1:1复刻。GNOME 3在更改操作逻辑的同时，受到了很多人的反对，MATE应运而生。  
MATE理所应当的使用了GTK框架，自定义程度类似Xfce4。  
默认主题是拟物风格，轻量但完全不及Xfce4，卖点是GNOME 2的1:1复刻。 
> 我不建议使用DeepinDesktopEnvironment或者是UbuntuKylinUI。  
> 这二者的优化十分的差劲，自定义程度甚至比GNOME还差，且不支持插件。  

---
## 其他窗口管理器
### WindowMaker/AfterStep
二者致力于还原[NeXTStep](https://m.wikipedia.org/wiki/NeXTSTEP)的使用体验，玩玩也挺好的:D  
### Enlightenment
特效十分充足的**仅支持Wayland**的堆叠式窗口管理器，配置差还想要炫酷特效的最佳选择。  
### FluxBox
嵌入式发行版TinyCoreLinux使用的窗口管理器，使用体验类似OpenBox，但是自定义不能。  
