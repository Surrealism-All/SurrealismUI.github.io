# SAvatar

SAvatar is a avatar component that defaults to Icons.Avatar when there are no images available

![](../../static/avatar.png)

## examples
```rust
import {SAvatar} from "../../index.slint";
import {ROOT-STYLES} from "../../themes/index.slint";

component TestWindow inherits Window {
  height: 400px;
  width: 400px;
  background: #F5F5F5;
  VerticalLayout {
    padding: 20px;
    spacing: 20px;
    SAvatar {
    }
    SAvatar {
      avatar-size : ROOT-STYLES.sur-size.small * 2;
      padding-type : Small;
      theme: Primary;
    }
    SAvatar {
      theme: Warning;
    }
    SAvatar {
      avatar-size : ROOT-STYLES.sur-size.small * 2;
      padding-type : Small;
      theme: Error;
    }
    SAvatar {
      avatar-size : ROOT-STYLES.sur-size.large * 2;
      padding-type : Large;
      theme: Dark;
      avatar:@image-url("../../README/imgs/logo.png");
    }
  }
}
```
## properties inherits SCard
- in property <length> avatar-size : avatar image size;
- in property <image> avatar : avatar image;
- in-out property <image> alt : if the image can be displayed the default alt will instead;
- in property <ImageFit> image-fit : image fit;