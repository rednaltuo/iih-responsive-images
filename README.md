With responsive imges, there's two problems we're trying to solve:

* Make images fit into mobile layouts while respecting their intrinsic size
* Avoid making the user download unnecessarily large image files

We accomplished the former by making images always stretch to fill 100% of their container while limiting their size with an inline max-width style. For the latter, we used srcset to optimize for screen resolution, srcset plus sizes to optimize for device width, and finally the <picture> element for manual control over which image file is displayed.
