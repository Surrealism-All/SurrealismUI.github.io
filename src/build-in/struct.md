# Struct Enum

## FontProps
- font-family (string) : font family
- font-size (length) : font size (16px👍)
- font-weight (int) : font weight [100,900] 500==Normal 
- font-italic (bool) : font italic
- color (brush) : font color
## ThemeColor
- light (ColorProps) : theme light
- primary (ColorProps) : theme primary
- success (ColorProps) : theme success
- info (ColorProps) : theme info
- warning (ColorProps) : theme warning
- error (ColorProps) : theme error
- dark (ColorProps) : theme dark
### ColorProps
- name (string) : color name
- weakest (brush) : weakest color
- weaker (brush) : weaker color
- normal (brush) : normal color
- deeper (brush) : deeper color
- deepest (brush) : deepest color
- font (brush) : font color
- opacity (brush) : opacity color
### ColorLevel
- Weakest
- Weaker
- Normal
- Deeper
- Deepest
- Font
- Opacity
## UseIcons (Global)
a quicker way to use SurrealismUI built in icons
- icons
## ThemePadding
- none (PaddingProps) : theme padding none
- tip (PaddingProps) : theme padding tip
- tag (PaddingProps) : theme padding tag
- icon (PaddingProps) : theme padding icon
- small (PaddingProps) : theme padding small
- normal (PaddingProps) : theme padding normal
- large (PaddingProps) : theme padding large
### PaddingProps 
- padding-top (length) : padding top
- padding-bottom: (length) : padding bottom
- padding-left (length) : padding left
- padding-right (length) : padding right
- padding-same (length) : padding
## ThemeBorder
- none (BorderProps) : no border 
- small (BorderProps) : small border 
- normal (BorderProps) : normal border 
- large (BorderProps) : large border 
- x-large (BorderProps) : x-large border 
- circle:`({
      none:BorderProps,
      small:BorderProps,
      normal:BorderProps,
      large:BorderProps,
      x-large:BorderProps,
    })` : circle border 
### BorderProps
- border-radius (length) : border radius
- border-width (length) : border width
- border-color (brush) : color of border
## SizeProps
- small (length) : size small
- normal (length) : size normal
- large (length) : size large
- largest (length) : size largest
## ThemeShadow
- low1 (ShadowProps) : lowest shadow
- low2 (ShadowProps) : lower shadow
- low3 (ShadowProps) : low shadow
- high1 (ShadowProps) : high shadow
- high2 (ShadowProps) : higher shadow
- high-empty (ShadowProps) : high blur but no x and y shadow
### ShadowProps
- x (length) : shadow x
- y (length) : shadow y
- blur (length) : shadow blur
## ThemeSpace
- none (length) : spacing when width == none(0px)
- len20 (length) : spacing when width == 20px
- len40 (length) : spacing when width == 40px
- len60 (length) : spacing when width == 60px
- len80 (length) : spacing when width == 80px
- len120 (length) : spacing when width == 120px
- len160 (length) : spacing when width == 160px
- len200 (length) : spacing when width == 200px
- len240 (length) : spacing when width == 240px
- len280 (length) : spacing when width == 280px
- len320 (length) : spacing when width == 320px
- len360 (length) : spacing when width == 360px
- len400 (length) : spacing when width == 400px
- len440 (length) : spacing when width == 440px
- len480 (length) : spacing when width == 480px
- len520 (length) : spacing when width == 520px
- len560 (length) : spacing when width == 560px
  
## SOption
```rust
export struct SOption {label:string,value:string}
```

## ResultType
```rust
export enum ResultType{
  Primary,
  Success,
  Info,
  Error,
  Warning,
  Help
}
```

## Position
```rust
export enum Position {
  Left,
  LeftTop,
  LeftBottom,
  Right,
  RightTop,
  RightBottom,
  Top,
  TopLeft,
  TopRight,
  Bottom,
  BottomLeft,
  BottomRight
}
```
## SDate
```rust
export struct SDate{
    year: int,
    month: int,
    day: int,
    hour: int,
    minute: int,
    second: int,
}
```
## SStepOption
```rust
export struct SStepOption {
  label: string,
  value: string,
  info: string,
}
```
---

## SAlertProps
```rust
export struct SAlertProps {
  font-weight : int,
  font-size: length,
  color : brush,
  font-italic : bool,
  font-family : string,
  overflow : TextOverflow,
  spacing : length,
  text : string,
  is-show : bool,
  alert-height : length,
  result-type: ResultType,
  close-icon : image,
  icon-size : length,
}
```
## SAvatarProps
```rust
export struct SAvatarProps {
  card-height : length,
  card-width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  avatar-size : length,
  avatar : image,
  alt : image,
  image-fit : ImageFit,
}
```
## SBadgeProps
```rust
export struct SBadgeProps {
  //font
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  //hight-width
  card-height : length,
  card-width : length,
  text : string,
  icon : image,
  position :Position,
  icon-color : brush,
}
```
## SButtonProps
```rust
export struct SButtonProps {
  font-weight : int,
  font-size : length,
  color : brush,
  font-italic : bool,
  font-family : string,
  theme : Themes,
  padding-type : PaddingType,
  shadow-type : ShadowType,
  border-type : BorderType,
  icon : image,
  show-icon : bool,
  text : string,
  letter-spacing : length,
  clip : bool,
  round : bool
}
```

## SCalendarProps
```rust
export struct SCalendarProps {
    //font
    font-weight : int,
    font-size: length,
    font-color : brush,
    font-italic : bool,
    font-family : string,
    //theme
    theme : Themes,
    //hight-width
    card-height : length,
    card-width : length,
    padding-type: PaddingType,
    shadow-type: ShadowType,
    border-type : BorderType,
    clip : bool,
    today: SDate,
    // zeller algorithm
    // https://en.wikipedia.org/wiki/Zeller%27s_congruence
    bg-visible : bool,
    active-date: SDate,
    current-date: SDate,
    months: [string],
    weekdays :[string],
  }
```

## SCardProps
```rust
export struct SCardProps {
  //font
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  //hight-width
  card-height : length,
  card-width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  clip : bool,
}
```

## SCollapseProps
```rust
export struct SCollapseProps {
  //font
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  //header
  header-height : length,
  header-title : string,
  header-padding-type: PaddingType,
  header-shadow-type: ShadowType,
  header-border-type : BorderType,
  //details
  details-height : length,
  details-padding-type: PaddingType,
  details-shadow-type: ShadowType,
  details-border-type : BorderType,
  is-show : bool,
  collapse-icon : image,
}
```
## SCarouselProps
```rust
export struct SCarouselProps {
    sources: [image],
    fold-strench: float,
    fold-width: length,
    fold-height: length,
    fit: ImageFit,
    focus-main: bool,
    active: int,
}
```

## SCheckboxProps
```rust
export struct SCheckboxProps {
  font-weight : int,
  font-size: length,
  color : brush,
  font-italic : bool,
  font-family : string,
  card-height : length,
  card-width : length,
  theme : Themes,
  active-color: brush,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  text : string,
  value : string,
  actived : bool,
  disabled : bool,
}
```

## SCollectionProps
```rust
export struct SCollectionProps {
  scale : float,
  is-scale : bool,
  easing : easing,
  duration : duration,
}
```
## SDialogProps
```rust
export struct SDialogProps {
  //theme
  theme : Themes,
  cancel-btn-theme : Themes,
  confirm-btn-theme : Themes,
  cancel-btn-text : string,
  confirm-btn-text : string,
  is-show: bool,
  mask-opacity : percent,
  spacing : length,
  //font
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //dialog
  dialog-theme : Themes,
  dialog-title : string,
  dialog-title-size : length,
  dialog-details : string,
  dialog-height : float,
  dialog-title-height : float,
  dialog-view-height : float,
  btn-view-height : float,
  dialog-width : float,
  dialog-details-padding-top : length,
  dialog-details-padding-bottom : length,
  dialog-details-padding-left : length,
  dialog-details-padding-right : length,
  dialog-details-alignment : LayoutAlignment,
  padding-type:PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
}
```
## SDividerProps
```rust
export struct SDividerProps {
  //theme
  theme : Themes,
  height : length,
  width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
}
```
## SDrawerProps
```rust
export struct SDrawerProps {
  theme : Themes,
  is-show : bool,
  mask-opacity : percent,
  padding-type: PaddingType,
  drawer-theme : Themes,
  position : Position,
  proportion : percent,
}
```
## FileItem
```rust
export struct FileItem {
  icon:image,
  name:string,
  datetime:string,
  file-type:string,
  size:string,
}
```
## SFileProps
```rust
export struct SFileProps {
  //theme
  theme : Themes,
  tabs : [SOption],
  column-width : [length],
  //tab
  font-family : string,
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  padding-type:PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  text-alignment: TextHorizontalAlignment,
  // item
  files : [FileItem],
  item-font-family : string,
  item-font-weight : int,
  item-font-size: length,
  item-font-italic : bool,
  item-padding-type:PaddingType,
}
```
## SHeaderProps
```rust
export struct SHeaderProps {
  spacing: length,
  source : image,
  options : [SOption],
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  //hight-width
  card-height : length,
  card-width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
}
```
## Icons
```rust
struct Icons {
  Null:image,
  Loading:image,
  Avatar:image,
  Success:image,
  Smiling_face:image,
  Info:image,
  Close_one:image,
  Attention:image,
  Help:image,
  Share:image,
  Up:image,
  Down:image,
  Down_one:image,
  Right:image,
  Right_one:image,
  Link_left:image,
  Preview_close:image,
  Preview_open:image,
  Close_one:image,
  Setting_two:image,
  Folder:image,
  Folder_filled:image,
  FileCode:image
}
```
## IconProps
```rust
struct IconProps {
  name:string,
  source:image
}
```
## SIconProps
```rust
struct SIconProps {
  mouse-cursor : MouseCursor,
  theme : Themes,
  height : length,
  width : length,
  padding : length,
  //image props
  source : image,
  colorize : brush,
  image-fit : ImageFit,
  image-rendering : ImageRendering,
  rotation : RotationProps,
  source-clip-x : int,
  source-clip-y : int,
  source-clip-height : int,
  source-clip-width : int
}
```
## SInputProps
```rust
export struct SInputProps {
  //font
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  //hight-width
  card-height : length,
  card-width : length,
  padding-type:PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  placeholder : string,
  disabled:bool,
  clearable:bool,
  //use eye-icon
  password:bool,
  has-focus:bool,
  type : InputType,
  icon-color : brush,
  text : string,
}
```
## KeyBoardType
```rust
export enum KeyBoardType {
    PhoneAlpha,
    PhoneNumber,
    Computer,
}
```
## SKeyItem
```rust
export struct SKeyItem {
    label: string,
    value: KeyItems
}
```
## SKeyBoardProps
```rust
export struct SKeyBoardProps {
    theme: Themes,
    font-size:length,
    keyboard-type: KeyBoardType,
}
```
## SLinkProps
```rust
export struct SLinkProps {
  icon : image,
  funny :  bool,
  underline : bool,
  mouse-cursor : MouseCursor,
  theme : Themes,
  font-size : length,
  text:string,
  font-weight : int,
  font-family : string,
  font-italic : bool,
}
```
## SLoadingProps
```rust
export struct SLoadingProps {
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  opacity : float,
  is-show : bool,
  theme : Themes,
  loading-icon : image,
  duration : duration,
  text : string,
  easing : easing,
  iteration-count : int,
}
```
## MenuData

```rust
export struct MenuData {
  id:string,
  icon : image,
  name : string,
}
```
## SMenuProps
```rust
export struct SMenuProps {
  theme : Themes,
  height : length,
  width :length,
  tip-width: length,
  icon-box-size : length,
  icon-size : length ,
  active : string,
  active-color : brush,
  menu-data : [MenuData],
  sub-menu-data : [MenuData],
  more-height : length, 
  more-width : length,
}
```
## SNumberInputProps
```rust
export struct SNumberInputProps {
  //font
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  //hight-width
  card-height : length,
  card-width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  clip : bool,
  minimum: float,
  maximum: float,
  value: float,
  disabled : bool,
  step : float,
  strict : bool,
  input-type : InputType,
}
```

## SPaginationProps
```rust
export struct SPaginationProps {
    theme: Themes,
    active: int,
    page-size: int,
    total: int,
    pre-icon: image,
    next-icon: image,
    size: length,
    visible-range: int,
}
```

## SPersonaProps
```rust
export struct SPersonaProps {
  btn-text : string,
  btns : [SButtonProps],
  //avatar
  avatar : image,
  avatar-height: length,
  avatar-theme : Themes,
  card-width : length,
  spacing : length,
  //name
  name : string,
  name-height: length,
  name-font-size: length,
  name-font-weight : int,
  name-theme: Themes,
  name-font-family: string,
  name-font-italic: bool,
  //des
  des : string,
  des-height: length,
  des-font-size: length,
  des-font-weight : int,
  des-theme: Themes,
  des-font-family: string,
  des-font-italic: bool,
}
```
## SPopoverProps
```rust
export struct SPopoverProps {
  theme : Themes,
  position : Position,
  is-show : bool,
  owner-height:length,
  owner-width:length
}
```

## SPopupProps
```rust
export struct SPopupProps {
  is-show : bool,
  theme : Themes,
  mask-opacity : percent,
}
```
## SProgressProps
```rust
export struct SProgressProps {
  //font
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  //hight-width
  height : length,
  width : length,
  text : string,
  progress : float,
}
```
## SRadioProps
```rust
export struct SRadioProps {
  font-weight : int,
  font-size: length,
  color : brush,
  font-italic : bool,
  font-family : string,
  card-height : length,
  card-width : length,
  theme : Themes,
  active-color: brush,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  text : string,
  value : string,
  actived : bool,
  disabled: bool,
}
```
## SResultProps
```rust
export struct SResultProps {
  card-height : length,
  card-width : length,
  icon-size : length,
  btns : [SButtonProps],
  btn-text : string,
  result-type: ResultType,
  text : string,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  icon : image,
  theme : Themes,
}
```
## SSelectProps
```rust
export struct SSelectProps {
  //font
  font-weight : int,
  font-size: length,
  font-italic : bool,
  font-family : string,
  item-font-weight : int,
  item-font-size: length,
  item-font-italic : bool,
  item-font-family : string,
  //theme
  theme : Themes,
  //hight-width
  card-height : length,
  card-width : length,
  padding-type:PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  options : [SOption],
  placeholder : string,
  is-show : bool,
}
```

## SStepProps
```rust
export struct SStepProps {
  theme : Themes,
  font-family : string,
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  active: int,
  active-color: brush,
  done-color: brush,
  undone-color: brush,
  options : [SStepOption],
}
```

## SSwitchProps
```rust
export struct SSwitchProps {
  //container
  card-height : length,
  card-width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  active : bool,
  theme: Themes,
  //switch-circle
  switch-height : length,
  switch-width : length,
  switch-padding-type: PaddingType,
  switch-shadow-type: ShadowType,
  switch-border-type : BorderType,
  switch-background-color : brush,
  switch-border-color : brush,
  switch-drop-shadow-color : color,
}
```
## SSwitchGroupProps
```rust
export struct SSwitchGroupProps {
  card-height : length,
  card-width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  active : string,
  theme: Themes,
  switchs : [SOption],
  font-family : string,
  font-weight : int,
  font-size: length,
  font-italic : bool,
}
```
## STabbarProps
```rust
export struct STabbarProps {
    //font
    font-weight: int,
    font-size: length,
    font-color : brush,
    font-italic : bool,
    font-family : string,
    //theme
    theme : Themes,
    //hight-width
    card-height : length,
    card-width : length,
    padding-type: PaddingType,
    shadow-type: ShadowType,
    border-type : BorderType,
    clip : bool,
    tabs: [MenuData],
    icon-scale: float,
    tab-size: length,
    active: int,
    show-text:bool,
}
```
## STableProps
```rust
export struct STableProps {
  //theme
  columns : [SOption],
  column-width : [length],
  column-themes:[Themes],
  viewport-height:length,
  //tab
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  //theme
  theme : Themes,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  alignment: TextHorizontalAlignment,
}
```
## STableColumnProps
```rust
export struct STableColumnProps {
  index : int,
  datas : [string],
  height : length,
  width : length,
  //tab
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  font-family : string,
  theme : Themes,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  alignment: TextHorizontalAlignment,
}
```
## STagProps
```rust
export struct STagProps {
  text : string,
  font-size : length,
  font-weight : int,
  font-family : string,
  font-italic : bool,
  theme : Themes,
  padding-type : PaddingType,
  border-type : BorderType,
  shadow-type : ShadowType
}
```
## STextProps
```rust
struct STextProps {
  font-family : string,
  font-weight : int,
  font-size : length,
  color : brush,
  font-italic : bool,
  theme : Themes,
  wrap :TextWrap,
  overflow : TextOverflow,
  letter-spacing : length,
  horizontal-alignment : TextHorizontalAlignment,
  vertical-alignment : TextVerticalAlignment,
}
```
## STipProps
```rust
export struct STipProps {
  //font
  font-family : string,
  font-weight : int,
  font-size: length,
  font-color : brush,
  font-italic : bool,
  //theme
  theme : Themes,
  wrap : TextWrap,
  overflow : TextOverflow,
  letter-spacing : length,
  horizontal-alignment : TextHorizontalAlignment,
  vertical-alignment : TextVerticalAlignment,
  position : Position,
  is-show : bool,
  text : string,
  tip-width : length,
}
```
## STreeProps
```rust
export struct STreeProps {
  //font
  font-family : string,
  font-weight : int,
  font-size: length,
  font-italic : bool,
  //font
  item-font-family : string,
  item-font-weight : int,
  item-font-size: length,
  item-font-italic : bool,
  //theme
  theme : Themes,
  //hight-width
  height : length,
  width : length,
  padding-type: PaddingType,
  shadow-type: ShadowType,
  border-type : BorderType,
  tree-data : TreeData
}
```
## STimeLineProps
```rust
export struct STimeLineProps {
    id: string,
    theme: Themes,
    date: string,
    header-alignment: TextHorizontalAlignment,
    font-size: length,
    active: bool,
}
```