# Square Sans

![image](https://github.com/aidrecabrera/square-sans/assets/61798731/63b6410a-c6f5-4398-aa7b-a6f305917d99)

I really love this font. So, I decided to save it in my Github for personal projects! 👀

Square Sans consists of two distinct styles: **Square Sans Text** and **Square Sans Display**. Each style offers different weights and variations to accommodate various design requirements.

### Disclaimer

Please note that the Square Sans are the property of Square and are subject to their terms of use. This guide is intended for personal and educational purposes only.

### 1. Square Sans Text

Square Sans Text is optimized for readability in smaller sizes, making it ideal for body text and UI elements. It offers the following styles:

- **Regular**: A standard weight for everyday use.
- **Medium**: A slightly heavier weight suitable for emphasis and headings.
- **Regular Italic**: An italic variation of the regular weight, providing a stylish touch to text.

### 2. Square Sans Display

Square Sans Display is tailored for larger sizes and headlines, enhancing visual impact. It includes the following style:

- **Regular**: A versatile weight designed for headlines and prominent text.

## Font Demo

You can access the font demo here: [Square Sans Demo](https://aidrecabrera.github.io/square-sans/index.html)

## Font Usage

To use Square Sans fonts in your projects, follow these steps:

1. **Download Fonts**: Obtain the font files from the this repository or Square's official website. [Guide here](#How-to-Obtain-through-Square).
2. **Include Fonts**: Include the font files in your project directory.
3. **Font-Face Declaration**: Declare the font faces in your CSS stylesheet using `@font-face` rules, specifying the font family, source URLs, weights, and styles.
4. **Apply Styles**: Apply the desired font family, weight, and style to your HTML elements using CSS properties such as `font-family`, `font-weight`, and `font-style`.

There is a stylesheet provided in the repository that you can use in your project.

## How to Obtain through Square

I obtained the fonts by accessing the Square Fonts CDN and retrieving the font files directly from the server. By inspecting the network requests while loading the Square website, the URLs for the font files were identified, allowing for direct download.

To obtain these fonts, follow these steps:

1. **Load Square's Website**: Navigate to [Square's website](https://squareup.com/).
   
2. **Open Developer Tools**: Open the browser's developer tools.

3. **Navigate to Network Tab**: Within the developer tools, navigate to the "Network" tab.

4. **Filter for Fonts**: In the "Network" tab, filter the requests by typing "font" in the filter input box.

5. **Find Font Requests**: Look through the requests to find the font files. The font files typically have a `.woff2` extension.

6. **Extract Font URL**: Click on the request corresponding to the font file you want to obtain. In the request details, you will find the "Request URL". Copy this URL.

7. **Download Font**: Paste the copied URL into your browser's address bar and press Enter. This should initiate the download of the font file.

8. **Repeat for Other Fonts**: Repeat steps 6 and 7 for each font variant you want to obtain.

![image](https://github.com/aidrecabrera/square-sans/assets/61798731/e61ac3a0-32f0-4c89-b902-806b9b6d12d9)


### Getting the Fonts Directly
The fonts can be obtained directly from the Square Fonts CDN:

- **Square Sans Text Upright**: [Download WOFF2](https://square-fonts-production-f.squarecdn.com/square-text/SquareSansText-Upright-VF.woff2)
- **Square Sans Text Medium**: [Download WOFF2](https://square-fonts-production-f.squarecdn.com/square-text/SquareSansText-Medium.woff2)
- **Square Sans Text Italic**: [Download WOFF2](https://square-fonts-production-f.squarecdn.com/square-text/SquareSansText-Italic-VF.woff2)
- **Square Sans Display**: [Download WOFF2](https://square-fonts-production-f.squarecdn.com/square-display/SquareSansDisplay-VF.woff2)

## Example Usage with Tailwind CSS

### CSS

```css
@font-face {
  font-family: "Square Sans Display";
  src: url("https://square-fonts-production-f.squarecdn.com/square-display/SquareSansDisplay-VF.woff2") format("woff2");
  font-weight: 100 900;
  font-style: normal;
}

@font-face {
  font-family: "Square Sans Text Italic";
  src: url("https://square-fonts-production-f.squarecdn.com/square-text/SquareSansText-Italic-VF.woff2") format("woff2");
  font-weight: 100 900;
  font-style: italic;
}

@font-face {
  font-family: "Square Sans Text Medium";
  src: url("https://square-fonts-production-f.squarecdn.com/square-text/SquareSansText-Medium.woff2") format("woff2");
  font-weight: 500;
  font-style: normal;
}

@font-face {
  font-family: "Square Sans Text Upright";
  src: url("https://square-fonts-production-f.squarecdn.com/square-text/SquareSansText-Upright-VF.woff2") format("woff2");
  font-weight: 100 900;
  font-style: normal;
}
```

### JavaScript (Tailwind Configuration)

```js
module.exports = {
  theme: {
    extend: {
      fontFamily: {
        "square-sans-display": ["Square Sans Display", "sans-serif"],
        "square-sans-text-italic": ["Square Sans Text Italic", "sans-serif"],
        "square-sans-text-medium": ["Square Sans Text Medium", "sans-serif"],
        "square-sans-text-upright": ["Square Sans Text Upright", "sans-serif"],
      },
    }
  }
}
```

### Usage

To use these fonts in your Tailwind CSS project, you can refer to them using the defined font family names:

```html
<div class="font-square-sans-display">This text uses Square Sans Display font.</div>
<div class="font-square-sans-text-italic">This text uses Square Sans Text Italic font.</div>
<div class="font-square-sans-text-medium">This text uses Square Sans Text Medium font.</div>
<div class="font-square-sans-text-upright">This text uses Square Sans Text Upright font.</div>
```

Make sure to include these font face declarations and Tailwind CSS configuration in your project setup. Adjust the URLs in the font face declarations as necessary to match the location of the font files in your project setup.

## Example Usage CSS

```css
@font-face {
    font-family: 'Square Sans Text';
    src: url('path/to/SquareSansText-RegularItalic.eot');
    font-weight: normal;
    font-style: italic;
}

.your-style {
    font-family: 'Square Sans Text';
    font-weight: normal;
    font-style: italic;
}
```

## Square Sans Demo

![image](https://github.com/aidrecabrera/square-sans/assets/61798731/dd293d1f-9266-4509-a5c9-5a0f53d6bb8b)
