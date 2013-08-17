threex.depthoffield
===================

Provide a tunable depth of field to your scene.
It gives it a nice [bokeh](http://en.wikipedia.org/wiki/Bokeh) effect.
It is very easy to include.
Additionally there is a
[Dat.GUI](https://code.google.com/p/dat-gui/)
helpers provided for interactive fine tuning.

Here is a [basic example](http://jeromeetienne.github.io/threex.depthoffield/examples/basic.html) and its [source](https://github.com/jeromeetienne/threex.depthoffield/blob/master/examples/basic.html).

How To Install It
=================

You can install it manually. Just do 

```html
<script src='threex.depthoffield.js'></script>
```

You can install with [bower](http://bower.io/).

```bash
bower install threex.depthoffield
```

then you add that in your html

```html
<script src="bower_components/threex.depthoffield/threex.depthoffield.js"></script>
```

How To Use It ?
===============

first you initialize it

```
var depthOfField= new THREEx.DepthOfField(renderer)
```

then you call this function everytime you want to render it

```
depthOfField.render(scene, camera)
```

Becareful with the camera far distance... it greatly affects the precision of the
```THREE.MeshDepthMaterial``` rendering. Keep it close to the minimum.

