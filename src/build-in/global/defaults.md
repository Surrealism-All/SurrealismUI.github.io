# DefaultProps

- default props can help you know `SurrealismUI` Widgets' props
- each widget has default prop
- so you can change the default prop to change the widget
- all default props are exported by schema
- you can find these default props in themes dir


## DefaultSAlertProps

```rust
export global DefaultSAlertProps {
  in-out property <int> font-weight : 700;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <TextOverflow> overflow : TextOverflow.elide;
  in-out property <length> spacing : 16px;
  in-out property <string> text : "this is a alert message!";
  in-out property <bool> is-show : false;
  in-out property <length> alert-height : font-size * 1.5;
  in-out property <ResultType> result-type: ResultType.Success;
  in-out property <image> close-icon : UseIcons.icons.Close-one;
  in-out property <length> icon-size : 16px;
}
```
## DefaultSAvatarProps

```rust
export global DefaultSAvatarProps {
  in-out property <length> card-height : avatar-size;
  in-out property <length> card-width : avatar-size;
  in-out property <PaddingType> padding-type: PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : Circle-Normal;
  in-out property <length> avatar-size : ROOT-STYLES.sur-size.normal * 2;
  in-out property <image> avatar;
  in-out property <image> alt : UseIcons.icons.Avatar;
  in-out property <ImageFit> image-fit : ImageFit.cover;
}
```
## DefaultSBadgeProps
```rust
export global DefaultSBadgeProps {
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size - 2px;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //hight-width
  in-out property <length> card-height : font-size;
  in-out property <length> card-width : font-size;
  in-out property <string> text : "";
  in-out property <image> icon : UseIcons.icons.Attention;
  in-out property <Position> position : Position.RightTop;
  in-out property <brush> icon-color : GlobalProps.font.color;
}
```
## DefaultSButtonProps
```rust
export global DefaultSButtonProps {
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  in property <PaddingType> padding-type:PaddingType.Normal;
  in property <ShadowType> shadow-type: ShadowType.Low1;
  in property <BorderType> border-type : BorderType.Normal;
  in property <image> icon;
  in property <bool> show-icon : false;
  in-out property <string> text : "SButton";
  in property <length> letter-spacing : GlobalProps.text-action.letter-spacing;
  in property <bool> clip : GlobalProps.clip;
  in property <bool> round : false;
}
```
## DefaultSCalendarProps

```rust
export global DefaultSCalendarProps {
    //font
    in-out property <int> font-weight : GlobalProps.font.font-weight;
    in-out property <length> font-size: GlobalProps.font.font-size;
    in-out property <brush> font-color : GlobalProps.font.color;
    in-out property <bool> font-italic : GlobalProps.font.font-italic;
    in-out property <string> font-family : GlobalProps.font.font-family;
    //theme
    in-out property <Themes> theme : GlobalProps.theme;
    //hight-width
    in-out property <length> card-height : GlobalProps.standard-height;
    in-out property <length> card-width : GlobalProps.standard-width;
    in-out property <PaddingType> padding-type:PaddingType.Normal;
    in-out property <ShadowType> shadow-type: ShadowType.Low1;
    in-out property <BorderType> border-type : BorderType.Normal;
    in-out property <bool> clip : GlobalProps.clip;
    in-out property <SDate> today;
    // zeller algorithm
    // https://en.wikipedia.org/wiki/Zeller%27s_congruence
    in property <bool> bg-visible : false;
    in-out property <SDate> active-date: today;
    in-out property <SDate> current-date: today;
    in-out property <[string]> months: ["Jan","Fab","Mar", "Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"];
    in-out property <[string]> weekdays : ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat","Sun"];
}
```

## DefaultSCardProps
```rust
export global DefaultSCardProps {
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //hight-width
  in-out property <length> card-height : GlobalProps.standard-height;
  in-out property <length> card-width : GlobalProps.standard-width;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
  in-out property <bool> clip : GlobalProps.clip;
}
```

## DefaultSCarouselProps

```rust
export global DefaultSCarouselProps {
    in-out property <[image]> sources;
    in property <float> fold-strench: 1.1;
    in property <length> fold-width: 42px;
    in property <length> fold-height: 108px;
    in property <ImageFit> fit: ImageFit.preserve;
    in property <bool> focus-main: false;
    in-out property <int> active: 0;
}
```

## DefaultSCheckboxProps

```rust
export global DefaultSCheckboxProps {
    in-out property <int> font-weight: GlobalProps.font.font-weight;
    in-out property <length> font-size: GlobalProps.font.font-size;
    in-out property <brush> color: GlobalProps.font.color;
    in-out property <bool> font-italic: GlobalProps.font.font-italic;
    in-out property <string> font-family: GlobalProps.font.font-family;
    in-out property <length> card-height: GlobalProps.font.font-size;
    in-out property <length> card-width: GlobalProps.font.font-size;
    in-out property <Themes> theme: GlobalProps.theme;
    in-out property <brush> active-color: GlobalProps.active-color;
    in-out property <PaddingType> padding-type: PaddingType.Icon;
    in-out property <ShadowType> shadow-type: ShadowType.Low1;
    in-out property <BorderType> border-type: BorderType.Small;
    in-out property <string> text: "SCheckbox";
    in-out property <string> value: "checkbox";
    in-out property <bool> actived: false;
    in-out property <bool> disabled: false;
}

```

## DefaultSCollapseProps
```rust
export global DefaultSCollapseProps {
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //header
  in-out property <length> header-height : GlobalProps.font.font-size;
  in-out property <string> header-title : "collapse";
  in-out property <PaddingType> header-padding-type:PaddingType.Normal;
  in-out property <ShadowType> header-shadow-type: ShadowType.Low1;
  in-out property <BorderType> header-border-type : BorderType.Normal;
  //details
  in-out property <length> details-height : 120px;
  in-out property <PaddingType> details-padding-type:PaddingType.Normal;
  in-out property <ShadowType> details-shadow-type: ShadowType.Low1;
  in-out property <BorderType> details-border-type : BorderType.Normal;
  in-out property <bool> is-show : false;
  in-out property <image> collapse-icon : UseIcons.icons.Right-one;
}
```
## DefaultSCollectionProps
```rust
export global DefaultSCollectionProps {
  in-out property <float> scale : 2;
  in-out property <bool> is-scale : false;
  in-out property <easing> easing : ease-in-out;
  in-out property <duration> duration : 200ms;
}
```
## DefaultSDialogProps
```rust
export global DefaultSDialogProps {
  //theme
  in-out property <Themes> theme : Dark;
  in-out property <Themes> cancel-btn-theme : Info;
  in-out property <Themes> confirm-btn-theme : Primary;
  in-out property <string> cancel-btn-text : "Cancel";
  in-out property <string> confirm-btn-text : "Confirm";
  in-out property <bool> is-show:false;
  in-out property <percent> mask-opacity : 80%;
  in-out property <length> spacing : 16px;
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //dialog
  in-out property <Themes> dialog-theme : Dark;
  in-out property <string> dialog-title : "Dialog Title";
  in-out property <length> dialog-title-size : 18px;
  in-out property <string> dialog-details : "This is a dialog info";
  in-out property <float> dialog-height : 0.36;
  in-out property <float> dialog-title-height : 0.2;
  in-out property <float> dialog-view-height : 0.6;
  in-out property <float> btn-view-height : 0.2;
  in-out property <float> dialog-width : 0.6;
  in-out property <length> dialog-details-padding-top : 0;
  in-out property <length> dialog-details-padding-bottom : 0;
  in-out property <length> dialog-details-padding-left : 0;
  in-out property <length> dialog-details-padding-right : 0;
  in-out property <LayoutAlignment> dialog-details-alignment : end;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
}
```
## DefaultSDividerProps
```rust
export global DefaultSDividerProps {
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <length> height : 2px;
  in-out property <length> width : 100%;
  in-out property <PaddingType> padding-type:PaddingType.None;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.None;
}
```
## DefaultSDrawerProps
```rust
export global DefaultSDrawerProps {
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <bool> is-show : false;
  in-out property <percent> mask-opacity : 80%;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <Themes> drawer-theme : Light;
  in-out property <Position> position : Left;
  in-out property <percent> proportion : 30%;
}
```
## DefaultSFileProps
```rust
export global DefaultSFileProps {
  //theme
  in-out property <Themes> theme :GlobalProps.theme;
  in-out property <[SOption]> tabs : [];
  in-out property <[length]> column-width : [];
  //tab
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : 700;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
  in-out property <TextHorizontalAlignment> text-alignment: TextHorizontalAlignment.left;
  // item
  in-out property <[FileItem]> files : [];
  in-out property <string> item-font-family : GlobalProps.font.font-family;
  in-out property <int> item-font-weight : GlobalProps.font.font-weight;
  in-out property <length> item-font-size: GlobalProps.font.font-size;
  in-out property <bool> item-font-italic : GlobalProps.font.font-italic;
  in-out property <PaddingType> item-padding-type:PaddingType.Normal;
}
```
## DefaultSHeaderProps
```rust
export global DefaultSHeaderProps {
  in-out property <length> spacing: 2px;
  in-out property <image> source :UseIcons.icons.Right;
  in-out property <[SOption]> options : [
    {label:"src",value:"src"},
    {label:"header",value:"header"},
    {label:"SHeader",value:"SHeader"}
  ];
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //hight-width
  in-out property <length> card-height : font-size;
  in-out property <length> card-width : GlobalProps.standard-width;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
}
```
## DefaultSIconProps
```rust
export global DefaultSIconProps {
  in-out property <MouseCursor> mouse-cursor : MouseCursor.pointer;
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <length> height : GlobalProps.standard-icon-size;
  in-out property <length> width : GlobalProps.standard-icon-size;
  in-out property <length> padding : 0;
  //image props
  in-out property <image> source;
  in-out property <brush> colorize;
  in property <ImageFit> image-fit : ImageFit.contain;
  in property <ImageRendering> image-rendering : ImageRendering.smooth;
  in-out property <RotationProps> rotation : {
    rotation-angle : 0,
    rotation-origin-x : 0,
    rotation-origin-y: 0,
  };
  in-out property <int> source-clip-x : 0;
  in-out property <int> source-clip-y : 0;
  in-out property <int> source-clip-height : 0;
  in-out property <int> source-clip-width : 0;
}
```
## DefaultSInputProps
```rust
export global DefaultSInputProps {
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //hight-width
  in-out property <length> card-height : font-size;
  in-out property <length> card-width : 18 * font-size;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
 
  in-out property <string> placeholder : "please input";
  in-out property <bool> disabled:false;
  in-out property <bool> clearable:false;
  //use eye-icon
  in-out property <bool> password:false;
  in-out property <bool> has-focus:false;
  in-out property <InputType> type : InputType.text;
  in-out property <brush> icon-color;
  in-out property <string> text :"";
}
```
## DefaultKeyBoardProps

```rust
export global DefaultKeyBoardProps {
    in property <Themes> theme: Themes.Dark;
    in property <length> font-size: 16px;
    in-out property <KeyBoardType> keyboard-type: KeyBoardType.PhoneNumber;
}
```

## DefaultSLinkProps
```rust
export global DefaultSLinkProps {
  in-out property <image> icon : UseIcons.icons.Share;
  in-out property <bool> funny :  false;
  in-out property <bool> underline : true;
  in-out property <MouseCursor> mouse-cursor : pointer;
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <length> font-size : GlobalProps.font.font-size;
  in-out property <string> text:"";
  in-out property <int> font-weight : 500;
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
}
```
## DefaultSLoadingProps
```rust
export global DefaultSLoadingProps {
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <float> opacity : 1;
  in-out property <bool> is-show : false;
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <image> loading-icon : UseIcons.icons.Loading;
  in-out property <duration> duration : 1200ms;
  in-out property <string> text : "Loading ...";
  in-out property <easing> easing : ease-in-out;
  in-out property <int> iteration-count : -1;
}
```
## DefaultSMenuProps

```rust
export global DefaultSMenuProps {
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <length> height : 100%;
  in-out property <length> width : 60px;
  in-out property <length> tip-width;
  in-out property <length> icon-box-size : 60px;
  in-out property <length> icon-size : GlobalProps.font.font-size * 2 ;
  in-out property <string> active : "0";
  in-out property <brush> active-color : GlobalProps.active-color;
  in-out property <[MenuData]> menu-data : [
    {id:"0",icon:UseIcons.icons.FileCode,name:"Code"},
    {id:"1",icon:UseIcons.icons.Search,name:"Search"},
    {id:"2",icon:UseIcons.icons.Help,name:"Help"},
  ];
  in-out property <[MenuData]> sub-menu-data : [
    {id:"2-1",icon:UseIcons.icons.Avatar,name:"User"},
    {id:"2-2",icon:UseIcons.icons.Setting-two,name:"Settings"}
  ];
  in-out property <length> more-height; 
  in-out property <length> more-width;
}
```
## DefaultSNumberInputProps
```rust
export global DefaultSNumberInputProps {
    //font
    in-out property <int> font-weight : GlobalProps.font.font-weight;
    in-out property <length> font-size: GlobalProps.font.font-size;
    in-out property <brush> font-color : UseSurrealismFn.get-color(root.theme, ColorLevel.Font);
    in-out property <bool> font-italic : GlobalProps.font.font-italic;
    in-out property <string> font-family : GlobalProps.font.font-family;
    //theme
    in-out property <Themes> theme : GlobalProps.theme;
    //hight-width
    in-out property <length> card-height : self.font-size;
    in-out property <length> card-width : GlobalProps.standard-width;
    in-out property <PaddingType> padding-type:PaddingType.Normal;
    in-out property <ShadowType> shadow-type: ShadowType.Low1;
    in-out property <BorderType> border-type : BorderType.Normal;
    in-out property <bool> clip : true;
    in-out property <float> minimum: 0;
    in-out property <float> maximum: 100;
    in-out property <float> value: 0;
    in-out property <bool> disabled : false;
    in property <float> step : 1.0;
    in property <bool> strict : false;
    in-out property <InputType> input-type : InputType.decimal;
}
```
## DefaultSPaginationProps

```rust
export global DefaultSPaginationProps {
    in property <Themes> theme: Themes.Dark;
    in-out property <int> active: 0;
    in property <int> page-size: 10;
    in property <int> total: 50;
    in property <image> pre-icon: UseIcons.icons.Left;
    in property <image> next-icon: UseIcons.icons.Right;
    in property <length> size: 18px;
    in property <int> visible-range: 5;
}
```

## DefaultSPersonaProps
```rust
export global DefaultSPersonaProps {
  in-out property <string> btn-text : "Click";
  in-out property <[SButtonProps]> btns : [];
  in-out property <image> avatar : @image-url("");
  in-out property <length> avatar-height:130px;
  in-out property <Themes> avatar-theme : GlobalProps.theme;
  in-out property <length> card-width : 200px;
  in-out property <length> spacing : 8px;
  //name
  in-out property <string> name : "SYF20020816";
  in-out property <length> name-height: GlobalProps.font.font-size * 3;
  in-out property <length> name-font-size: GlobalProps.font.font-size + 2px;
  in-out property <int> name-font-weight : 700;
  in-out property <Themes> name-theme: GlobalProps.theme;
  in-out property <string> name-font-family : GlobalProps.font.font-family;
  in-out property <bool> name-font-italic : GlobalProps.font.font-italic;
  //des
  in-out property <string> des : @tr("A Rust | Vue Developer\nEmail:\nsyf20020816@outlook.com");
  in-out property <length> des-height: des-font-size * 1.5 * 3;
  in-out property <length> des-font-size: GlobalProps.font.font-size - 2px;
  in-out property <int> des-font-weight : GlobalProps.font.font-weight;
  in-out property <Themes> des-theme: GlobalProps.theme;
  in-out property <string> des-font-family : GlobalProps.font.font-family;
  in-out property <bool> des-font-italic : GlobalProps.font.font-italic;
}
```

## DefaultSPopoverProps
```rust
export global DefaultSPopoverProps {
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <Position> position : Position.Top;
  in-out property <bool> is-show : false;
  in-out property <length> owner-height;
  in-out property <length> owner-width;
}
```

## DefaultSPopupProps
```rust
export global DefaultSPopupProps {
  in-out property <bool> is-show : false;
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <percent> mask-opacity : 80%;
}
```
## DefaultSProgressProps
```rust
export global DefaultSProgressProps {
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size - 2px;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //hight-width
  in-out property <length> height : 8px + font-size * 2;
  in-out property <length> width : 100%;
  in-out property <string> text : @tr("now: {}%" , round(progress * 100));
  in-out property <float> progress : 0;
  in-out property <length> stroke-width: 8px;
  in-out property <brush> stroke-color;
  in property <bool> circle:false;
}
```
## DefaultSRadioProps
```rust
export global DefaultSRadioProps {
    in-out property <int> font-weight: GlobalProps.font.font-weight;
    in-out property <length> font-size: GlobalProps.font.font-size;
    in-out property <brush> color: GlobalProps.font.color;
    in-out property <bool> font-italic: GlobalProps.font.font-italic;
    in-out property <string> font-family: GlobalProps.font.font-family;
    in-out property <length> card-height: GlobalProps.font.font-size;
    in-out property <length> card-width: GlobalProps.font.font-size;
    in-out property <Themes> theme: GlobalProps.theme;
    in-out property <brush> active-color: GlobalProps.active-color;
    in-out property <PaddingType> padding-type: PaddingType.Icon;
    in-out property <ShadowType> shadow-type: ShadowType.Low1;
    in-out property <BorderType> border-type: BorderType.Small;
    in-out property <string> text: "SRadio";
    in-out property <string> value: "radio";
    in-out property <bool> actived: false;
    in-out property <bool> disabled: false;
}
```
## DefaultSResultProps
```rust
export global DefaultSResultProps {
  in-out property <length> card-height : 200px;
  in-out property <length> card-width : 140px;
  in-out property <length> icon-size : 48px;
  in-out property <[SButtonProps]> btns : [];
  in-out property <string> btn-text : "CLICK!";
  in-out property <ResultType> result-type:ResultType.Success;
  in-out property <string> text : "This is a success message!";
  in-out property <PaddingType> padding-type: PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
  in-out property <image> icon : UseIcons.icons.Success;
  in-out property <Themes> theme : Success;
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> color : ROOT-STYLES.sur-theme-colors.success.font;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
}
```
## DefaultSSelectProps
```rust
export global DefaultSSelectProps {
  //font
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> item-font-weight : GlobalProps.font.font-weight;
  in-out property <length> item-font-size: GlobalProps.font.font-size;
  in-out property <bool> item-font-italic : GlobalProps.font.font-italic;
  in-out property <string> item-font-family : GlobalProps.font.font-family;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //hight-width
  in-out property <length> card-height : font-size;
  in-out property <length> card-width : 180px;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
  in-out property <[SOption]> options;
  in-out property <string> placeholder : "please select";
  in-out property <bool> is-show : false;
}
```
## DefaultSSwitchProps
```rust
export global DefaultSSwitchProps {
  //container
  in-out property <length> card-height : 6px;
  in-out property <length> card-width : 24px;
  in-out property <PaddingType> padding-type: PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Small;
  in-out property <bool> active : false;
  in-out property <Themes> theme:GlobalProps.theme;
  //switch-circle
  in-out property <length> switch-height : 6px + ROOT-STYLES.sur-padding.normal.padding-same;
  in-out property <length> switch-width : 6px + ROOT-STYLES.sur-padding.normal.padding-same;
  in-out property <PaddingType> switch-padding-type: PaddingType.None;
  in-out property <ShadowType> switch-shadow-type: ShadowType.Low1;
  in-out property <BorderType> switch-border-type : Normal;
  in-out property <brush> switch-background-color : ROOT-STYLES.sur-theme-colors.dark.deepest;
  in-out property <brush> switch-border-color : ROOT-STYLES.sur-theme-colors.dark.deepest;
  in-out property <color> switch-drop-shadow-color : ROOT-STYLES.sur-theme-colors.dark.weakest;
}
```
## DefaultStepProps
```rust
export global DefaultStepProps {
  in property <Themes> theme : Dark;
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <int> active: 1;
  in property <brush> active-color: ROOT-STYLES.sur-theme-colors.primary.normal;
  in property <brush> done-color: ROOT-STYLES.sur-theme-colors.success.normal;
  in property <brush> undone-color: ROOT-STYLES.sur-theme-colors.dark.normal;
  in property <[SStepOption]> options : [];
}
```

## DefaultSSwitchProps

```rust
export global DefaultSSwitchProps {
  //container
  in-out property <length> card-height : 6px;
  in-out property <length> card-width : 24px;
  in-out property <PaddingType> padding-type: PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Small;
  in-out property <bool> active : false;
  in-out property <Themes> theme:GlobalProps.theme;
  //switch-circle
  in-out property <length> switch-height : 6px + ROOT-STYLES.sur-padding.normal.padding-same;
  in-out property <length> switch-width : 6px + ROOT-STYLES.sur-padding.normal.padding-same;
  in-out property <PaddingType> switch-padding-type: PaddingType.None;
  in-out property <ShadowType> switch-shadow-type: ShadowType.Low1;
  in-out property <BorderType> switch-border-type : Normal;
  in-out property <brush> switch-background-color : ROOT-STYLES.sur-theme-colors.dark.deepest;
  in-out property <brush> switch-border-color : ROOT-STYLES.sur-theme-colors.dark.deepest;
  in-out property <color> switch-drop-shadow-color : ROOT-STYLES.sur-theme-colors.dark.weakest;
}
```

## DefaultSSwitchGroupProps
```rust
export global DefaultSSwitchGroupProps {
  in-out property <Themes> theme:GlobalProps.theme;
  in-out property <length> card-height : self.font-size / 2;
  in-out property <length> card-width : 140px;
  in-out property <PaddingType> padding-type: PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.None;
  in-out property <string> active ;
  in-out property <[SOption]> switchs : [];
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: 14px;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
}
```
## DefaultSTableProps
```rust
export global DefaultSTableProps {
  //theme
  in-out property <Themes> theme :GlobalProps.theme;
  in-out property <[SOption]> columns : [];
  in-out property <[length]> column-width : [];
  in-out property <[Themes]> column-themes:[];
  in-out property <length> viewport-height;
  //tab
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : 700;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.None;
  in-out property <TextHorizontalAlignment> alignment: TextHorizontalAlignment.left;
}
```
## DefaultSTableColumnProps
```rust
export global DefaultSTableColumnProps {
  //theme
  in-out property <Themes> theme :GlobalProps.theme;
  in-out property <int> index;
  in-out property <[string]> datas;
  in-out property <length> height;
  in-out property <length> width;
  //tab
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.None;
  in-out property <TextHorizontalAlignment> alignment: TextHorizontalAlignment.left;
}
```
## DefaultSTagProps
```rust
export global DefaultSTagProps {
  in-out property <string> text : "";
  in property <length> font-size : ROOT-STYLES.tag-size;
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  in-out property <PaddingType> padding-type : PaddingType.Tag;
  in-out property <BorderType> border-type : BorderType.Normal;
  in-out property <ShadowType> shadow-type : ShadowType.Low1;
  in-out property <Themes> theme : GlobalProps.theme;
}
```
## DefaultSTextProps
```rust
export global DefaultSTextProps {
  //font
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <TextWrap> wrap :GlobalProps.text-action.wrap;
  in-out property <TextOverflow> overflow : GlobalProps.text-action.overflow;
  in-out property <length> letter-spacing : GlobalProps.text-action.letter-spacing;
  in-out property <TextHorizontalAlignment> horizontal-alignment : GlobalProps.text-alignment.horizontal-alignment;
  in-out property <TextVerticalAlignment> vertical-alignment : GlobalProps.text-alignment.vertical-alignment;
}
```

## DefaultSTimeLineProps

```rust
export global DefaultSTimeLineProps {
    in property <string> id;
    in property <Themes> theme: GlobalProps.theme;
    in property <string> date;
    in property <TextHorizontalAlignment> header-alignment: TextHorizontalAlignment.center;
    in property <length> font-size: 14px;
    in-out property <bool> active;
}
```

## DefaultSTipProps
```rust
export global DefaultSTipProps {
  //font
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : GlobalProps.font.font-weight;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <brush> font-color : GlobalProps.font.color;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  in-out property <TextWrap> wrap :word-wrap;
  in-out property <TextOverflow> overflow : GlobalProps.text-action.overflow;
  in-out property <length> letter-spacing : GlobalProps.text-action.letter-spacing;
  in-out property <TextHorizontalAlignment> horizontal-alignment : GlobalProps.text-alignment.horizontal-alignment;
  in-out property <TextVerticalAlignment> vertical-alignment : GlobalProps.text-alignment.vertical-alignment;
  in-out property <Position> position : Top;
  in-out property <bool> is-show : false;
  in-out property <string> text : "default tips";
  in-out property <length> tip-width : 0;
}
```
## DefaultSTreeProps
```rust
export global DefaultSTreeProps {
  //font
  in-out property <string> font-family : GlobalProps.font.font-family;
  in-out property <int> font-weight : 700;
  in-out property <length> font-size: GlobalProps.font.font-size;
  in-out property <bool> font-italic : GlobalProps.font.font-italic;
  //font
  in-out property <string> item-font-family : GlobalProps.font.font-family;
  in-out property <int> item-font-weight : GlobalProps.font.font-weight;
  in-out property <length> item-font-size: GlobalProps.font.font-size - 2px;
  in-out property <bool> item-font-italic : GlobalProps.font.font-italic;
  //theme
  in-out property <Themes> theme : GlobalProps.theme;
  //hight-width
  in-out property <length> height : 100%;
  in-out property <length> width : 100%;
  in-out property <PaddingType> padding-type:PaddingType.Normal;
  in-out property <ShadowType> shadow-type: ShadowType.Low1;
  in-out property <BorderType> border-type : BorderType.Normal;
  in-out property <TreeData> tree-data : {
    icon : UseIcons.icons.Folder,
    label: "parent_folder",
    extra:"",
    children:[
      {
        icon:UseIcons.icons.FileCode,
        label:"slint.slint",
        extra:"12KB", 
      },
      {
        icon:UseIcons.icons.FileCode,
        label:"surrealism.slint",
        extra:"126KB", 
      }
    ]
  };
}
```
