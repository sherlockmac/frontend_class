# Typography

## Importance of Typography
### 1. Readability
Readability is how easily text can be read.
**[Medium](https://medium.com/)** uses clean sans-serif fonts and adequate line spacing, enhancing readability.
- **Key Factors:**
    - **Font Choice:** Sans-serif for screens (e.g., Arial).
    - **Font Size:** Ensures legibility; too small frustrates users.
    - **Contrast:** High contrast, like black text on a white background, is crucial.
### 2. Aesthetics
Aesthetics refer to visual appeal.
**[Apple](https://www.apple.com/)** utilizes a modern typography style that complements its sleek design.
- **Key Factors:**
    - **Hierarchy:** Different sizes guide attention (e.g., large headings for key info).
    - **Consistency:** Uniform font usage creates cohesion.
    - **Style:** Typography reflects the brand’s personality, affecting first impressions.
### 3. Branding
Branding creates a unique identity.
**[Coca-Cola](https://www.coca-cola.com/)** uses its iconic script font, reinforcing its nostalgic brand image.
- **Key Factors:**
    - **Font Selection:** Reflects brand characteristics (e.g., elegant serifs for luxury).
    - **Logo Design:** Typography is integral to logo recognition.
    - **User Recognition:** Consistent typography enhances brand recall.
 
## CSS Properties
1. **font-family:**  
   Specifies the typeface for the text, allowing for custom font choices.  
   ```css
   font-family: 'Roboto', sans-serif;
   ```
2. **font-size:**  
   Sets the size of the text, influencing readability and layout.  
   ```css
   font-size: 16px;
   ```
3. **font-weight:**  
   Defines the thickness of the text, ranging from light to bold.  
   ```css
   font-weight: 700;
   ```
4. **line-height:**  
   Controls the vertical space between lines of text, enhancing readability.  
   ```css
   line-height: 1.5;
   ```
5. **letter-spacing:**  
   Adjusts the space between individual letters, affecting text appearance.  
   ```css
   letter-spacing: 0.05em;
   ```
6. **text-align:**  
   Determines the horizontal alignment of text (left, right, center, justify).  
   ```css
   text-align: center;
   ```
7. **text-transform:**  
   Changes the case of text, such as making it uppercase or lowercase.  
   ```css
   text-transform: uppercase;
   ```
8. **text-decoration:**  
   Adds decorative effects to text, like underlining or strikethrough.  
   ```css
   text-decoration: underline;
   ```
9. **text-shadow:**  
   Applies shadow effects to text, creating depth and visual interest.  
   ```css
   text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
   ```
10. **word-spacing:**  
    Modifies the space between words, impacting text flow and readability.  
    ```css
    word-spacing: 0.2em;
    ```
11. **color:**  
    Sets the color of the text, affecting visibility and aesthetics.  
    ```css
    color: #333;
    ```
12. **font-style:**  
    Applies styles like italic or oblique to the text for emphasis.  
    ```css
    font-style: italic;
    ```
13. **font-variant:**  
    Adjusts the font to display features like small caps.  
    ```css
    font-variant: small-caps;
    ```
14. **white-space:**  
    Controls how whitespace is handled in text, such as preventing wrapping.  
    ```css
    white-space: nowrap;
    ```
15. **overflow-wrap:**  
    Determines how text wraps within its container, especially for long words.  
    ```css
    overflow-wrap: break-word;
    ```
16. **text-overflow:**  
    Manages how overflowed text is displayed, such as using ellipsis for truncation.  
    ```css
    text-overflow: ellipsis;
    ```
17. **font-size-adjust:**  
    Allows adjustment of font sizes for better visual consistency across different fonts.  
    ```css
    font-size-adjust: 0.5;
    ```
18. **visibility:**  
    Controls the visibility of an element, allowing it to be hidden while still occupying space.  
    ```css
    visibility: hidden;
    ```
 
## How to Use Google Fonts
1. **Visit Google Fonts:**
   - Go to the [Google Fonts website](https://fonts.google.com).
2. **Choose a Font:**
   - Browse or search for a font you like. Click on it to see more details.
3. **Select Styles:**
   - After choosing a font, select the styles you want (like regular, bold, italic). Click the "+" button to add it to your selection.
4. **Open the Selected Fonts:**
   - A panel will appear at the bottom of the page. Click on it to view your selected fonts.
5. **Copy the Embed Code:**
   - In the panel, you'll see an `<link>` tag under "Embed." Copy this link.
6. **Add to Your HTML:**
   - Paste the `<link>` tag inside the `<head>` section of your HTML file:
     ```html
     <head>
       <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
     </head>
     ```
7. **Use the Font in CSS:**
   - In your CSS file, apply the font to elements using the `font-family` property:
     ```css
     body {
       font-family: 'Roboto', sans-serif;
     }
     ```
     
## BYOF (Bring Your Own Fonts)
To embed your own fonts in CSS, you can use the `@font-face` rule. Here’s how to do it:
1. **Upload Your Font Files:** Ensure your font files (e.g., .woff, .woff2, .ttf, .eot).
2. **Use the `@font-face` Rule:** Define the font in your CSS using the `@font-face` rule.
```css
@font-face {
    font-family: 'MyCustomFont'; /* Name of the font */
    src: url('fonts/MyCustomFont.woff2') format('woff2'), /* Modern browsers */
         url('fonts/MyCustomFont.woff') format('woff'),   /* Older browsers */
         url('fonts/MyCustomFont.ttf') format('truetype'); /* Legacy support */
    font-weight: normal; /* Font weight */
    font-style: normal;  /* Font style */
}

body {
    font-family: 'MyCustomFont', sans-serif; /* Use the custom font */
}
```
- **font-family:** Name you want to use for the font.
- **src:** Paths to the font files, with formats specified for better browser compatibility.
- **font-weight:** Indicates the weight of the font (normal, bold, etc.).
- **font-style:** Indicates the style (normal, italic, etc.).


## Best Practices
### 1. Keep it Simple and Legible
**[The Guardian](https://www.theguardian.com)** uses a clean sans-serif font for its articles, with clear headings and ample white space, making the content easy to read without distractions.
### 2. Use a Limited Number of Font Families
**[Dropbox](https://www.dropbox.com)** utilizes only two font families—one for headings and another for body text. This consistency helps create a cohesive brand identity and enhances user experience.
### 3. Maintain Consistent Spacing and Alignment
**[Stripe](https://stripe.com)** maintains consistent padding and margins across its site. Text elements are well-aligned, providing a structured and organized layout that enhances readability.
### 4. Contrast Between Text and Background
**[CNN](https://www.cnn.com)** features a dark text color on a light background, providing strong contrast that enhances visibility and allows users to easily read the content.

Google analyzes text contrast using the **Web Content Accessibility Guidelines (WCAG)**, specifically focusing on the contrast ratio between text and background colors.
### Key Metrics:
- **Contrast Ratio:** Ranges from 1:1 (no contrast) to 21:1 (maximum contrast). 
  - **4.5:1** is the minimum for normal text.
  - **3:1** is sufficient for large text (over 18pt or 14pt bold).
### Tools:
- **Lighthouse** in Chrome DevTools checks contrast ratios and highlights accessibility issues.
- **[WebAIM's Contrast Checker](https://webaim.org/resources/contrastchecker/)** is an online tool that allows users to input color values and see their contrast ratio.
