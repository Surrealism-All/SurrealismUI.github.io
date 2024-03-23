# SStar

SStar is a scoring component

## example
```rust
import {SStar,SButton} from "../../index.slint";
import {Themes,UseIcons} from "../../use/index.slint";

component TestWindow inherits Window {
  height: 400px;
  width: 400px;
  SStar {
    y: 20px;
  }
  hs:=SStar {
    score: 2.2;
    y: 60px;
    theme: Error;
    
  }
  SButton {
    y: 320px;
    x:10px;
    text: "add half";
    clicked => {
      hs.add-half();
    }
  }
  SStar {
    score : 3.8;
    disabled: true;
    y: 100px;
    theme: Success;
  }
  os:=SStar {
    max-score : 7;
    score : 2.8;
    y: 140px;
    theme: Info;
  }
  SButton {
    y: 320px;
    x: 115px;
    text: "add one";
    clicked => {
      os.add-one();
    }
  }
  fs:=SStar {
    max-score : 10;
    score : 7.2;
    y: 180px;
    no-theme:true;
    clicked(whole,half) => {
      t.n = whole;
      t.m = half;
    }
  }
  SButton {
    y: 320px;
    x: 220px;
    text: "get A";
    clicked => {
      fs.full();
    }
  }
  SButton {
    y: 320px;
    x: 305px;
    text: "clear";
    clicked => {
      fs.clear();
    }
  }
  t:=Text{
    y: 250px;
    font-size: 18px;
    in-out property <int> n;
    in-out property <int> m;
    text: "whole stars:"+ n + " half stars:" + m;
  }
}
```
## properties
- in property <bool> no-theme : use Surrealism Theme or not
- in property <float> score : the real score
- in property <Themes> theme : Themes.Primary;
- in property <bool> disabled : can be scored if disabled is false
- in property <float> max-score : max score (how many stars you wanna show)
## functions
- pure function get-half-stars()->bool : count the number of half stars ⛔
- pure function get-whole-stars()->int : count the number of whole stars ⛔
- pure function get-empty-stars()->int : count the number of empty stars ⛔
- public function full() : star all 👍
- public function clear() : no star 👍
- public function add-one() : add one star 👍
- public function add-half() : add half stars 👍
## callbacks
- callback clicked(float,float) : get how many whole stars and half stars
