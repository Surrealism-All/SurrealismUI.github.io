# Quickstart

<p style="color: #FB3746;font-weight: 700;">
If you use Cargo-Generate to build your project, you can skip this!<br>
Cargo Generate is a recommend way!
</p>

## Config SurrealismUI as Library (optional)

1. Open VsCode and choose Settings , then search `Slint:Library Paths`
2. Choose edit in settings.json
3. Find `slint.libraryPaths` and add `"SurrealismUI":"parent_file_path\\surrealism-ui\\index.slint"`❗

```json
  "slint.libraryPaths": {
    "SurrealismUI":"E:\\test_try\\test-surrealism\\ui\\modules\\surrealism-ui\\index.slint"
  },
```

<img src="./static/config.png" />

## Import and Use

```rust
import { SMenu,SCard,SHeader,SIcon,SButton  } from "../index.slint";
import {UseIcons } from "../use/index.slint";
import { STip } from "../src/tip/index.slint";
import { STag } from "../src/tag/index.slint";
import { SAlert } from "../src/alert/index.slint";

export component App inherits Window {
    height: 600px;
    width: 800px;
    private property <int> router-index : 0;
    HorizontalLayout {
      left-wrapper:=Rectangle {
        z: 111;
        height: 100%;
        width: menu.width;
        clip: false;
        menu:=SMenu {
          change(index,data) => {
            debug(index);
          }
        }
      }
      right-wrapper:=Rectangle {
        z: 100;
        width: parent.width - menu.width;
        background: #2b2b32;
        if router-index==0:index-page:= Rectangle {
            height: 100%;
            width: 100%;
            VerticalLayout {
              HorizontalLayout {
                padding: 8px;
                alignment: center;
                Rectangle {
                  height:header.height ;
                  width: parent.width - 16px;
                  header:=SHeader {
                    value: [{label:"SurrealismUI",value:"1"},{label:"menu:Index",value:"2"}];
                  }
                }
              }
              HorizontalLayout {
                padding: 24px;
                alignment: space-around;
                STag {
                  theme: Warning;
                  text: "SurrealismUI V0.3.3";
                }
                STag {
                  theme: Success;
                  text: "MIT License";
                }
                STag {
                  theme: Error;
                  text: "For Slint!";
                }
                STag {
                  theme: Error;
                  text: "author:syf20020816@outlook.com";
                }
              }
              HorizontalLayout {
                alignment: center;
                SCard {
                  card-width: 460px;
                  card-height: 320px;
                  SIcon {
                    height: parent.height;
                    width: parent.width;
                    source: @image-url("../README/imgs/logo.png");
                  }
                }
              }
              HorizontalLayout {
                padding: 24px;
                alignment: space-around;
                SButton {
                  text: "Try SurrealismUI";
                  clicked => {
                    alert.success("Try SurrealismUI!!! Let's GO!");
                  }
                }

                SButton {
                  show-icon: true;
                  icon: UseIcons.icons.Smiling-face;
                  theme: Primary;
                  text: "Star on Github!";
                }
                STip {
                  text: "GO TO SurrealismUI WIKI?\n Click here!";
                  height: wiki-btn.height;
                  width: wiki-btn.width;
                  position: Bottom;
                  wiki-btn:=SButton {
                    theme: Success;
                    text: "Read Wiki!~~~";
                    clicked => {
                      parent.clicked();
                    }
                  }
                }
              }

            }
        }
      }
    }
    alert:=SAlert {
      result-type: Success;
      text: "";
    }
}
```

<img src="./static/quickstart.png">