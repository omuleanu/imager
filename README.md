download dll [here](https://imager.codeplex.com/downloads/get/1569524)

add using:
``` ruby
using Omu.Drawing;
```

#### cropping
``` ruby
Image img = Imager.Crop(sourceImage, new Rectangle(x, y, width, height));
```

#### resizing
resize an image and maintain aspect ratio
``` ruby
Image img = Imager.Resize(sourceImage, newWidth, maxHeight, onlyResizeIfWider);
```

#### save
``` ruby
Imager.Save(path, img, Imager.GetEncoderInfo("image/gif"));
// image/gif is the MIME type for gif`
```

#### save as jpeg
``` ruby
Imager.SaveJpeg(path, img);
```

#### put on canvas
the image remains the same size, and it is placed in the middle of the new canvas
``` ruby
Imager.PutOnWhiteCanvas(img, width, height))
// or
Imager.PutOnCanvas(img, width, height, Color.White))
```

