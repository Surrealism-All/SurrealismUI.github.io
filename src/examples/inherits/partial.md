# Partial Inherits(部分继承)

this way always use when a widget has init callback

the new widget inherits default widget, it has default widget properties

use this way, you can add properties you need

```rust
component MyLabel2 {
  in property <int> default_font_weight: 500;
  SText {
    font-weight: default_font_weight;
    text:"partial inherits";
    font-size: 18px;
  }
}
```