# Related Products and Your Outfit
## Related Products
![Related_Products_Gif](https://media.giphy.com/media/QXIr8Tu7ANVZL8dWAs/giphy.gif)
### Scrollable list of product cards
  This feature was implemented by identifying the div that contained the carousel, and utilizing scrollLeft or scrollRight depending on which button was clicked.
### Feature comparison table
  On click on the star icon in the top right corner of each product card, a modal pops up which contains a dynamically rendered comparison table. This table compares the clicked on product to the main product. Each product has a list of features, but no two products are guaranteed to have the same type or number of features.

  The table utilizes a CSS grid to create the column layout. I formatted the data into an array and dynamically rendered it into the grid layout.
### Conditionally rendered scroll buttons
  The left and right buttons will only appear when there are products to the left or the right. On load, the div containing the carousel is inspected, and if there is overflow, the right arrow appears. Everytime a user clicks the left or right arrow, the carousel div is inspected for overflow. Once there are no more products to the left or right, the corresponding arrow disappears.

## Your Outfit List

### Add current product to Your Outfit list
  On click of the "Add to Your Outfit" tile, the main product will be added to the Your Outfit list. This information is prepared on load, so the addition will happen instantaneously on user click. Once a product has been added once, it can not be added again. This is done by saving all products in a Set. This prevents dupicates.

### Delete product from Your Outfit list
  On click of the X icon, a product will be removed from the list. This action removes the product from the Your Outfit Set. After this, a user is able to re-add a product to their outfit.

### General
  The Your Outfit list also utilizes a scrollable list of products and conditionally rendered scroll buttons. The implementation of these features is described in the Related Products section above.
