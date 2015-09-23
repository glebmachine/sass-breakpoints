# sass-breakpoints
Few mediaqueries, makes developers life a little bit easier

# avaliable mixins
**width-lessthan($max)**.

**width-morethan($min)**.

**width-between($min, $max)**.

**height-lessthan($max)**.

**height-morethan($min)**.

**height-between($min, $max)**.

# example
```sass

.header
  height : 60px
  
  +height-morethan(800)
    height : 80px

.layout
  width : 960px
  margin : 0 auto

  +width-between(640, 1000)
    width : auto
    padding : 0 20px
    
  +width-lessthan(620, 640)
    width : 600px
    padding : 0
    margin : 0 auto
  
  +width-lessthan(620)
    width : auto
    padding : 0 10px
```
