# All Inherits (全继承)

Inherit all properties of the widget, the new widget can use all origin widget properties

you can add more props in new widget

this is a common way, most of widgets can use this way

## example

```rust
component MyLabel1 inherits SText{
  in property <int> other_prop: 1;
  text: "all inherits";
  color: dodgerblue;
  font-weight: 700;
  font-size: 18px;
}
```