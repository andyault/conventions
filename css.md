# css

all css should be written with sass (scss). 

for rule methodologies, [bem](http://getbem.com/) should be used.

I'll be surprised if I ever finish this.

## directory structure
* style.scss
* modules/
  * _variables.scss 
  * _typography.scss
  * _boxmodel.scss
* lib/
  * [normalize.css](https://github.com/necolas/normalize.css/)
* elements/
* pages/

## file structure
```
//variables
$fontBody: helvetica, arial, sans-serif;

//blocks
.body {
  font-family: $fontBody;
}

//elements
.link {
  text-decoration: none;
}

//modifiers
.link-accent {
  color: $col2;
}

//animations
@keyframes {}
```

## property order
```
.class {
  //positioning
  content: ;
  position: ;
  display: ;
  width/height: ;
  top/right/bottom/left: ;
  justify-content/align-items/align-self: ;
  margin: ;
  padding: ;
  overflow: ;
  z-index: ;
  
  //style
  font/font-family/font-size/font-weight/font-style: ;
  text-align: ;
  line-height: ;
  text-transform/text-decoration: ;
  color: ;
  background: ;
  border/border-width/border-color/border-style/border-radius: ;
  
  //animations/transitions
  animation/animation-name/animation-duration: ;
  transition/transition-property/transition-duration: ;
  
  //pseudo classes (scss)
  &:hover {}
  
  //pseudo elements
  &::after {}
}
```
  
