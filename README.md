# Easter Animation 2026
jQuery UI Easter animation

## HTML/CSS
- `container`:
  - `aura`:
  - `hills`:
    - 3x divs styled using `hill`.
    - `cross`, contains HTML crucifix.
    - `shadow`, contains HTML crucifix.
## CSS (functional properties only)
- `container`:
  - `overflow`: makes sure that unneeded parts of `aura` and `hills` are visually cut out.
- `aura`:
  - `background-image`: set to a repeating conical gradient of yellows and oranges
  - `width` and `height`: set to larger than `container`.
  - `margin-left` and `margin-top`: offset to left and top to overlap `container` completely.
- `rotated` and `unrotated`:
  - `transform`: rotate either 0 or 360 degrees
  - `transition`: smooth animation, slow down at the end
-  `hills`:
  - `position` and `z-index`: set to be always above `container`. Important once animation begins.
  - `margin-top`: affects vertical positioning 
-  `hill`:
  - `border-radius`: for rounded corners of "hill".
  - `width` and `height`: same for squaring.
  - `transform`: rotate to diamond shape
  - `margin-top` and `margin-left`: depends on which "hill"
-  `cross` and `shadow`:
  - `margin-top`: depends which "crucifix". 

## jQuery / jQuery UI
- use `toggleClass()` on `aura`, toggling between `unrotated` and `rotated`.
- use jQueryUI's "puff" effect on `shadow`.

