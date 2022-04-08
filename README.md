# spark-shopify-carousel
1. Replace everything in your 'product-thumbnails.liquid' file in the Shopify Theme Editor with the contents in the 'product-thumbnails.liquid' file in this GitHub Repo.
2. Add (don't replace) the code from the Github Repo file: 'main-product--default.liquid' to the bottom of your 'main-product--default.liquid' file in the Shopify Theme Editor.

To add the functionality of showing the variant name (above the swatches) that has been clicked, add the following code (in bold) in between this section of 'main-product--default.liquid':
<label class="product__label {{ label_classes }}" for="Option{{ option.position }}">
  Selected {{ option.name }}:
  **<div class="variant_name"></div>**
</label>
