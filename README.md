rgb2gray
================

<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

## Install

`pip install rgb2gray`

<!-- ![image.png](images/ds.jpg)-->

## How to use

An example with
[`rgb2gray`](https://camille1.github.io/rgb2gray/converters.html#rgb2gray)
package.

``` python
from PIL import Image
import matplotlib.pyplot as plt
```

``` python
result = rgb2gray(Image.new('RGB', (10, 10), color = (255,255,0)))
result
```

    array([[226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226],
           [226, 226, 226, 226, 226, 226, 226, 226, 226, 226]], dtype=uint8)

``` python
plt.imshow(result, cmap='gray')
plt.show();
```

![](index_files/figure-gfm/cell-4-output-1.png)

``` python
img = Image.open('images/ds.jpg')
fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(15,10))

axes[0].imshow(img)
axes[1].imshow(rgb2gray(img), cmap='gray')
plt.show();
```

![](index_files/figure-gfm/cell-5-output-1.png)
