# Lecture 145. Image Optimisations

The image dimensions and the file size in term of killobites (kb) should be optimised for the web.

## hero.png

Reduce the intrinic size to 1200px width.
The current file size is 2mb which is too much.

To find out the size of the entire page:
Inspect UI -> Network tab, reload page -> Bottom-left: 4.5 mb transferred. This is too mch.

## Webp format image

A high performing image format to be able to really compress down images.

To compress a file or reduce the file size we use the [Squoosh website App](www.squoosh.app).

- upload the image.
- On the left is the original image and on the right is the compressed version.
- Use the Compress dropdown to select Browser PNG as we need to keep the transparent background.
- Edit image size: Compress -> OxiPNG, Effort -> 6. Now size is 482 kb which is small enough.
- Download image and rename to: hero-min.png
- Update index.html file.
  Test in UI:
- The file size has reduced to 3kb but the quality of image is not great.
- Go back to Squoosh site and change PNG to WebP. Find the balance between the image quality and the decompression.
- Checked with the [Can I Use](https://caniuse.com/) site and found that not all versions of Safari and Firefox fully support webp format. Therefore write the picture tag with x2 source tags. One ofr the webp and the other for the png. This will allow the browsers which one it can display.

Most modern version browsers can render webp format images but we use the picture tag with source tag inside to be on safe side. We still need the image tag.

hero-min.png -> the version that most browsers should be able to render.

## Conclusion

Now we can see how important it is to compress images to optimise them for the web.
