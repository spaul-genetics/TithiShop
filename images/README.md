# Product Images Directory

This directory is for storing product photos that will be displayed in the slideshow on the website.

**Note:** Sample placeholder images have been created (product1.jpg through product5.jpg). You can replace these with your actual product photos.

## How to Add Images

1. Add your product images to this `images` directory
2. Name them as follows:
   - `product1.jpg` (or `.png`)
   - `product2.jpg`
   - `product3.jpg`
   - `product4.jpg`
   - `product5.jpg`

3. Supported formats: `.jpg`, `.jpeg`, `.png`, `.webp`

## Tips

- **Recommended image size:** 800px - 1200px wide
- **File size:** Keep images under 2MB for faster loading
- **Aspect ratio:** 4:3 or 16:9 works best
- The slideshow will automatically hide any images that don't exist
- You can add more than 5 images by editing `index.qmd` and adding more slide divs

## Adding More Images

If you want to add more than 5 images:

1. Open `index.qmd`
2. Find the slideshow section
3. Add more `<div class="slide">` elements with your image paths
4. Add corresponding dots in the `.slideshow-dots` section

Example:
```html
<div class="slide">
  <img src="images/product6.jpg" alt="Product Image 6" onerror="this.style.display='none';">
</div>
```

And add a dot:
```html
<span class="dot" onclick="currentSlide(6)"></span>
```

