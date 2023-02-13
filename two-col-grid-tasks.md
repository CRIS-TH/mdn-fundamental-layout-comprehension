# Fundamental Layout Comprension Tutorial

## Create Layout: Two Column Grid

### Tasks

1. To display the navigation items *in a row*, with an *equal amount of space*
   between the items.

   **Resources**

   * [Setting display: flex](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Introduction#setting_display_flex)
   * [Flexbox: Horizontal and Vertical Alignment](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox#horizontal_and_vertical_alignment)

   Make the `ul` a *flex container*.
   In `styles.css`, add this to the selector body (but do no remove the other attributes).

   ```css
   nav ul {
      /* existing attributes ... */

      /* make this a flex container */
      display: flex;

      /* list items equally spaced: align centered horizontally and vertically */
      align-items: center;
      justify-content: space-between;
   }
   ```

1. The navigation bar should scroll with the content and then become stuck at the top of the viewport when it reaches it.

   **Resources**

   * [Sticky positioning](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning#sticky_positioning)

   ```css
   nav {
      /* existing attributes ... */

      /* scroll with content, then stick to the top left */ 
      position: sticky;
      top: 0px;
      left: 0px;
   }
   ```

   You probably will want to duplicate (copy/paste) the paragraphs to create
   enough scrollable content to test the sticky navigation bar.

1. The image that is inside the article should have text wrapped around it.

   **Resources**

   * [Floats](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Floats)

   ```css
   .feature {
      /* existing attributes ... */

      /* float image to the left inside block of text */
      float: left;

      /* margin: top right bottom left */
      margin: 0 1em 1em 0;
   }
   ```

1. The `<article>` and `<aside>` elements should display as a two column layout.
   The columns should be a flexible size so that if the browser window
   shrinks smaller the columns become narrower.

   **Resources**

   * [Flexible grids with the fr unit](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids#flexible_grids_with_the_fr_unit)

   ```css
   .grid {
      /* existing attributes ... */

      /* two column layout with first column 3 times larger (proportionally) */
      display: grid;
      grid-template-columns: 3fr 1fr;
   }
   
   main article {
      /* a little padding looks nice */
      padding-right: 1em;
   }

   ```

1. The photographs should display as a two column grid with a 1 pixel gap
   between the images.

   **Resources**

   * [Gaps between tracks](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids#gaps_between_tracks)

   ```css
   .photos {
      /* existing attributes ... */

      /* two column grid with 1px gap */
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1px;
   }
   ```
