### Painting with differentiable topologies and light: reconstructing physics from camera image without data(sets)

Can also work like NeRF but from one image. Use 3D Gaussians as light and assortments of shapes whose topologies can change.

Then trace (optimize) that light to the pixels of a camera to optimize MSE of image.

Due to light's physics being inductively defined, a 3D scene is optimized from just one image. Topologies can be variously shapeable/positioned 3D Gaussians.

Same methods can of course be used for reverse engineering crystalline structures from one XRD pattern.

No radiance fields. Actual physics. e.g. maybe Gaussian splatting (read paper) but with actual physics and formulation for differentiable in-world topologies?

---

just saving since had this idea before Gaussian splatting came out (still haven't read the paper), described with a much larger scope in mind elsewhere in this repo [here](https://github.com/animal-tree/Writing-stuff-2/blob/main/Theories/Old-summaries/Differentiable-universe-my-old-MHDPA-concept.md), [here](https://github.com/animal-tree/Writing-stuff-2/blob/main/Theories/Old-summaries/Theory-of-everything.md), and [here](https://github.com/animal-tree/Writing-stuff-2/blob/main/Theories/Colossal-Misery.md).

(haven't read any NeRF papers either. I was conceptualizing the Gaussian version of this before NeRFs became popularized)
