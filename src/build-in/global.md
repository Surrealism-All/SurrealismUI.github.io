# Global

## ROOT_STYLES

Root Theme Styles

- out property <FontProps> sur-font : SurrealismUI default font styles
- in-out property <length> tag-size : tag size to `STag`
- out property <brush> font-light : font color - light #fff
- out property <brush> font-black : font color - black #000
- in-out property <ThemeColor> sur-theme-colors : SurrealismUI theme colors
- in-out property <brush> radio-active : radio active color
- out property <ThemePadding> sur-padding : theme padding
- out property <ThemeBorder> sur-border : theme border
- out property <{low:{shadow1:percent,shadow2:percent},high:{shadow1:percent,shadow2:percent}}> sur-opacity : theme opacity
- out property <duration> sur-an-duration : theme animation duration
- out property <easing> sur-an-easing : theme animation easing
- in-out property <SizeProps> sur-size : the size of components
- out property <length> scroll-bar-width : scroll bar width
- out property <ThemeShadow> sur-shadow : theme shadow
- out property <ThemeSpace> sur-spacing : theme spacing

### source code

```rust
export global ROOT_STYLES {
  out property <FontProps> sur-font:{
    font-family:"Arial",
    font-weight:400,
    font-size:16px,
    font-italic:false,
  };
  in-out property <length> tag-size : 12px;
  out property <brush> font-light : #ffffff;
  out property <brush> font-black : #000;
  in-out property <ThemeColor> sur-theme-colors : {
    light:{name:"light",weakest:#F6F6F6,weaker:#E0E0E0,normal:#FFFFFF,deeper:#F5F5F5,deepest:#C8C8C6,font:#212121,opacity:#E0E0E088},
    primary:{name:"primary",weakest:#88D0EC,weaker:#6CB8F7,normal:#3AA1F5,deeper:#1891F3,deepest:#0B86F1,font:#e5ffff,opacity:#3AA1F588},
    success:{name:"success",weakest:#8FCEC4,weaker:#61BF84,normal:#38A762,deeper:#21964A,deepest:#118A3D,font:#e5fffb,opacity:#38A76288},
    info:{name:"info",weakest:#F6F6F6,weaker:#eaeaea,normal:#E0E0E0,deeper:#D2D2D2,deepest:#BDBDBD,font:#484848,opacity:#E0E0E088},
    warning:{name:"warning",weakest:#ffd5bd,weaker:#FCBD99,normal:#F9A677,deeper:#F9955C,deepest:#F8894A,font:#fff4ec,opacity:#F9A67788},
    error:{name:"error",weakest:#e9a7a7,weaker:#f48989,normal:#ed5e5e,deeper:#ed4e4e,deepest:#ed3b3b,font:#ffe5e4,opacity:#ed4e4e88},
    dark:{name:"dark",weakest:#707070,weaker:#616161,normal:#3a3a3a,deeper:#242424,deepest:#000000,font:#e4e4e4,opacity:#42424288}
  };
  in-out property <brush> radio-active : #FF9248;
  out property <ThemePadding> sur-padding : {
    none:{
      padding-top:0,
      padding-bottom:0,
      padding-left:0,
      padding-right:0,
      padding-same:0
    },
    tag:{
      padding-top:4px,
      padding-bottom:4px,
      padding-left:6px,
      padding-right:6px,
      padding-same:5px
    },
    icon:{
      padding-top:2px,
      padding-bottom:2px,
      padding-left:2px,
      padding-right:2px,
      padding-same:2px
    },
    tip:{
      padding-top:6px,
      padding-bottom:6px,
      padding-left:10px,
      padding-right:10px,
      padding-same:8px
    },
    small: {
      padding-top:8px,
      padding-bottom:8px,
      padding-left:12px,
      padding-right:12px,
      padding-same:10px
    },
    normal:{
      padding-top:10px,
      padding-bottom:10px,
      padding-left:16px,
      padding-right:16px,
      padding-same:14px
    },
    large:{
      padding-top:16px,
      padding-bottom:16px,
      padding-left:24px,
      padding-right:24px,
      padding-same:20px
    }
  };
  
  out property <ThemeBorder> sur-border:{
    none:{border-radius:0px,border-width:0px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
    small:{border-radius:2px,border-width:1px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
    normal:{border-radius:4px,border-width:2px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
    large:{border-radius:8px,border-width:4px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
    x-large:{border-radius:12px,border-width:6px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
    circle:{
      none:{border-radius:1000in,border-width:0px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
      small:{border-radius:1000in,border-width:1px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
      normal:{border-radius:1000in,border-width:2px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
      large:{border-radius:1000in,border-width:4px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
      x-large:{border-radius:1000in,border-width:6px,border-color:ROOT-STYLES.sur-theme-colors.dark.normal},
    }
  };
  out property <{
    low:{shadow1:percent,shadow2:percent},
    high:{shadow1:percent,shadow2:percent}
  }> sur-opacity : {
    low:{shadow1:28%,shadow2:14%},
    high:{shadow1:28%,shadow2:20%}
  };
  out property <duration> sur-an-duration :200ms;
  out property <easing> sur-an-easing : ease-in-out;
  in-out property <SizeProps> sur-size:{
    small:12px,
    normal:16px,
    large:24px,
    largest:48px
  };
  out property <length> scroll-bar-width : 14px;
  out property <ThemeShadow> sur-shadow:{
    low1:{x:0,y:1px,blur:2px},
    low2:{x:0,y:2px,blur:4px},
    low3:{x:0,y:4px,blur:8px},
    high1:{x:0,y:4px,blur:14px},
    high2:{x:0,y:8px,blur:28px},
    high-empty:{x:0,y:0px,blur:28px}
  };
  out property <ThemeSpace> sur-spacing:{
    none:0,
    len20:2px,
    len40:4px,
    len60:6px,
    len80:8px,
    len120:12px,
    len160:16px,
    len200:20px,
    len240:24px,
    len280:28px,
    len320:32px,
    len360:36px,
    len400:40px,
    len440:44px,
    len480:48px,
    len520:52px,
    len560:56px,
  };
}

```

## GlobalProps

default global properties

- in-out property <FontProps> font
- in-out property <Themes> theme
- in-out property <TextActionProps>
- in property <TextAlignmentProps> text-alignment
- in-out property <length> line-height
- in-out property <length> standard-height
- in-out property <length> standard-width
- in-out property <length> standard-icon-size
- in-out property <bool> clip
- in-out property <brush> active-color

### source code

```rust
export global GlobalProps {
  /**global font style */
  in-out property <FontProps> font : {
    font-family : ROOT-STYLES.sur-font.font-family,
    font-size : ROOT-STYLES.sur-font.font-size,
    font-weight : ROOT-STYLES.sur-font.font-weight,
    font-italic : ROOT-STYLES.sur-font.font-italic,
    color : ROOT-STYLES.sur-theme-colors.dark.font
  };
  /**global theme */
  in-out property <Themes> theme : Themes.Dark;
  in-out property <TextActionProps> text-action : {
    wrap : TextWrap.word-wrap,
    overflow : TextOverflow.elide,
    letter-spacing : 0,
  };
  in property <TextAlignmentProps> text-alignment : {
    horizontal-alignment : TextHorizontalAlignment.left,
    vertical-alignment : TextVerticalAlignment.center,
  };
  in-out property <length> line-height : ROOT-STYLES.sur-font.font-size * 1.5;
  in-out property <length> standard-height : UseSurrealismFn.count-height(line-height,ROOT-STYLES.sur-padding.normal.padding-top);
  in-out property <length> standard-width : UseSurrealismFn.count-width(ROOT-STYLES.sur-font.font-size,ROOT-STYLES.sur-padding.normal.padding-left);
  in-out property <length> standard-icon-size : ROOT-STYLES.sur-font.font-size;
  in-out property <bool> clip : true;
  in-out property <brush> active-color : ROOT-STYLES.radio-active;
}
```

## UseIcons (Global)

a quicker way to use SurrealismUI built in icons

- icons