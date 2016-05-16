# regl-smooth-life

> SmoothLife on the GPU, via regl

A quick implementation of SmoothLife on the GPU using [regl](https://github.com/mikolalysenko/regl). GPGPU has never been so easy. As far as WebGL goes, this is little more than a trivial modification of Mikola's [Game of Life](https://github.com/mikolalysenko/regl/blob/gh-pages/example/life.js) example.

It's pretty inefficient since it's brute-forcing the convolution. It's unrolling the loop as intelligently as possible, but really need to figure out GPU FFT. It might actually be faster to do this in plain js, but it was a great REGL learning experience.

See demo at: [http://rickyreusser.com/regl-smooth-life](http://rickyreusser.com/regl-smooth-life)

But for a better implementation, see: [smoothnacl](https://github.com/binji/smoothnacl/) from the [PNaCl Demos](https://gonativeclient.appspot.com/demo) site.

### References

Rafler, Stephan (2011). "[Generalization of Conway's "Game of Life" to a continuous domain - SmoothLife](http://arxiv.org/abs/1111.1567)". [arXiv:1111.1567v2](http://arxiv.org/abs/1111.1567).

### License

&copy; 2016 Ricky Reusser. MIT License.
