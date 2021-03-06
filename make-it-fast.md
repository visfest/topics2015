
# Make it fast

Why is D3 slow? Is it really slow? Or are you trying to show too many data points? The latter is a visualization problem, not a technological one.

The next version of D3, v4, you could use a lot of the features of D3 without the selection. You can use a fake DOM. YOu can use WebGL. 

React is building a shadow DOM and it tries to be smart about how you apply it to the real time. You can do the same thing with canvas.

If you care about making it fast, you just use webGL. You could also just use the parts that don't deal with the DOM like layouts.

There are a lot of multi-target renders. I can think of maybe 5 or 6. You can write them once and say "I want it as a canvas or SVG".

Who wants to make vis fast and why is it slow now?

One techniques for rendering large data sets is to render in chunks.

Have you ever played around with Web Workers?

http://papaparse.com/ was mentioned has being useful for chunking

If you want to render a lot of points all at the same time, webGL / OpenGL might be useful.

What is WebGL ? It's way to talk to GPUs for doing computations in parallel

GPGPU can also be used to do computations other than graphics in parallel

[Shader School](https://github.com/stackgl/shader-school) is a nice first place to learn more about WebGL / Shaders

[X3Dom](http://www.x3dom.org/)

[PIXIjs](http://www.pixijs.com/) A nice library that uses WebGL for 2D graphics so you don't have to.

Strategies for speeding up visualizations that don't require a technical approach?

**Link to BigVis?**

Sometimes you don't know what is the question. You don't even know if you expect to see an outliner. That's a case where you cannot filter, where you cannot have an aggregation.

Another technique: Start loading the filters the user is likely to click on before the do.
