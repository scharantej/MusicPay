## Flask Application Design

**Problem:** Build a website for downloading music files on payment in user location currency.

**Solution:**

### HTML Files

1. `index.html`:
   - Homepage for the website.
   - Contains information about the website and the music available for download.
   - Includes links to the music listing and checkout pages.

2. `music_listing.html`:
   - Displays the list of available music files.
   - Each music file should include its title, artist, album, genre, and price.
   - Users can click on a music file to view its details or add it to their cart.

3. `checkout.html`:
   - Allows users to review their cart and make a payment.
   - Includes fields for entering payment information, such as credit card number, expiration date, and CVV code.
   - Also contains a currency converter to convert the price to the user's local currency.

4. `confirmation.html`:
   - Displayed after a successful payment.
   - Contains a link to download the music files purchased.

### Routes

1. `/`:
   - Route for the homepage.
   - Returns the `index.html` file.

2. `/music-listing`:
   - Route for displaying the list of music files.
   - Returns the `music_listing.html` file.

3. `/checkout`:
   - Route for the checkout page.
   - Returns the `checkout.html` file.

4. `/confirmation`:
   - Route for displaying the order confirmation page.
   - Returns the `confirmation.html` file.

5. `/purchase`:
   - Route for processing the payment and downloading the music files.
   - Accepts payment information and converts the price to the user's local currency.
   - Generates a link for downloading the music files.

6. `/about`:
   - Route for displaying information about the website and its developers.
   - Returns a static HTML page.

7. `/contact`:
   - Route for displaying a contact form.
   - Returns a static HTML page with a form that allows users to send a message to the website administrators.