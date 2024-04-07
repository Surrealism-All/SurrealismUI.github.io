# SCarousel
The Carousel component is designed to display a sequence of images (or slides) that users can navigate through. It provides a dynamic and visually engaging way to showcase multiple images without occupying too much space on the screen.
## example

### focus main

![](../../static/carousel1.gif)
```rust
component TestCarousel {
    height: 400px;
    width: 600px;
    Rectangle {
        SCarousel {
            height: 300px;
            width: 100%;
            active: 3;
            focus-main: true;
            sources: [
                @image-url("../../README/imgs/sed1.jpeg"),
                @image-url("../../README/imgs/sed2.jpeg"),
                @image-url("../../README/imgs/sed3.png"),
                @image-url("../../README/imgs/sed4.png"),
                @image-url("../../README/imgs/sed5.png")
            ];
        }
    }
}
```
### normal

![](../../static/carousel2.gif)
```rust
component TestCarousel2 {
    height: 400px;
    width: 600px;
    Rectangle {
        SCarousel {
            height: 300px;
            width: 100%;
            active: 1;
            sources: [
                @image-url("../../README/imgs/sed1.jpeg"),
                @image-url("../../README/imgs/sed2.jpeg"),
                @image-url("../../README/imgs/sed3.png"),
                @image-url("../../README/imgs/sed4.png"),
                @image-url("../../README/imgs/sed5.png")
            ];
        }
    }
}
```

## Properties
- `in-out property <[image]> sources` : An array of images that the carousel will display. This property can be both read and set, allowing dynamic update of the carousel's content.
- `in property <float> fold-strench` : A float value that determines the stretching effect of non-central folds/slides. It defaults to `DefaultSCarouselProps.fold-stretch`, which should be a predefined value in your system.
- `in property <length> fold-width` : Specifies the width of each fold/slide in the carousel. It uses a length value and defaults to `DefaultSCarouselProps.fold-width`.
- `in property <length> fold-height` : Determines the height of the folds/slides. By default, it matches the height of the root component (`root.height`).
- `in property <ImageFit> fit` : Defines how images should be fitted within their frames, utilizing predefined `ImageFit` options. It defaults to `DefaultSCarouselProps.fit`.
- `in property <bool> focus-main` : A boolean indicating whether the main (center) image should be focused. Defaults to `DefaultSCarouselProps.focus-main`.
- `in-out property <int> active` : An integer representing the currently active slide. It starts from `0` and can be read or set to change the active slide.
## Callbacks
- `callback clicked(int)` : This callback is triggered when a slide is clicked. It passes the index of the clicked slide as an argument, allowing for custom interaction handling, such as navigating to a specific slide or performing an action related to the clicked slide's content.
