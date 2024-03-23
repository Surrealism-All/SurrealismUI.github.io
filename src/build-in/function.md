# Function

## `UseSurrealismFn`
- pure public function count-height(h:length,padding:length)->length : count component height
- pure public function count-width(w:length,padding:length)->length : count component weight
- pure public function get-padding(size:PaddingType)->PaddingProps : get padding by PaddingType
- pure public function get-shadow(shadow:ShadowType)->ShadowProps : get shadow by ShadowType
- pure public function get-shadow-x(shadow:ShadowType)->length : get shadow x by ShadowType
- pure public function get-shadow-y(shadow:ShadowType)->length : get shadow y by ShadowType
- pure public function get-shadow-blur(shadow:ShadowType)->length : get shadow blur by ShadowType
- pure public function get-border(border:BorderType)->BorderProps : get border by BorderType
- pure public function get-space(w:length) -> length : get spacing by component width
- pure public function deeper(theme:Themes,color:brush)->brush : get deeper theme color
  - pure public function light-deeper(color:brush)->brush : get deeper light theme color
  - pure public function primary-deeper(color:brush)->brush : get deeper primary theme color
  - pure public function success-deeper(color:brush)->brush : get deeper success theme color
  - pure public function info-deeper(color:brush)->brush : get deeper info theme color
  - pure public function warning-deeper(color:brush)->brush : get deeper warning theme color
  - pure public function error-deeper(color:brush)->brush : get deeper error theme color
  - pure public function dark-deeper(color:brush)->brush : get deeper dark theme color
- pure public function get-color(theme:Themes,level:ColorLevel)->brush : get color by theme and ColorLevel
  - pure public function get-color-light(level:ColorLevel)->brush : get light color by ColorLevel
  - pure public function get-color-dark(level:ColorLevel)->brush : get dark color by ColorLevel
  - pure public function get-color-primary(level:ColorLevel)->brush : get primary color by ColorLevel
  - pure public function get-color-info(level:ColorLevel)->brush : get info color by ColorLevel
  - pure public function get-color-warning(level:ColorLevel)->brush : get warning color by ColorLevel
  - pure public function get-color-success(level:ColorLevel)->brush : get success color by ColorLevel
  - pure public function get-color-error(level:ColorLevel)->brush : get error color by ColorLevel