# sanatana-awakening




























This is a detailed explanation of each line of your code:  

---

### **HTML Structure Explanation**

#### **Document Declaration & Head Section**
```html
<!DOCTYPE html>
<html lang="en">
```
- `<!DOCTYPE html>`: Defines the document type as HTML5.
- `<html lang="en">`: Starts the HTML document and sets the language to English.

```html
<head>
    <meta charset="UTF-8">
```
- `<head>`: Contains metadata and external resource links.
- `<meta charset="UTF-8">`: Ensures proper encoding to display special characters correctly.

```html
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- Ensures responsive design by setting the viewport width to match the device's width.

```html
    <title>Sanatana Awakening</title>
```
- Sets the browser tab title to "Sanatana Awakening."

```html
    <link href="https://fonts.googleapis.com/css2?family=Merienda&display=swap" rel="stylesheet">
```
- Imports the "Merienda" font from Google Fonts.

```html
    <link rel="stylesheet" href="styles.css">
</head>
```
- Links an external stylesheet (`styles.css`) for styling.

---

### **Body Section**

```html
<body>
```
- Starts the content of the webpage.

#### **Navigation Bar (Header Section)**
```html
<nav class="navbar">
    <div class="logo">Sanatana Awakening</div>
```
- `<nav>`: Creates a navigation bar.
- `<div class="logo">`: Displays the website name as a logo.

```html
    <ul class="nav-links" id="navLinks">
```
- `<ul>`: Creates a list of navigation links.

```html
        <li><a href="#">Home</a></li>
        <li><a href="#">Courses</a></li>
        <li><a href="#">Books</a></li>
        <li><a href="#">History</a></li>
        <li><a href="#">Ancient Tech</a></li>
        <li><a href="#">Blogs</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
```
- Each `<li>` (list item) contains an `<a>` (anchor) tag linking to different sections.

```html
    </ul>
```
- Closes the navigation list.

#### **Login & Sign Up Buttons**
```html
    <div class="nav-buttons">
        <a href="#" class="btn login">Login</a>
        <a href="#" class="btn signup">Sign Up</a>
    </div>
```
- Two buttons: "Login" and "Sign Up" with CSS classes (`btn`, `login`, `signup`).

#### **Hamburger Menu for Mobile**
```html
    <div class="hamburger" onclick="toggleMenu()">☰</div>
</nav>
```
- `<div class="hamburger">☰</div>`: Creates a hamburger menu.
- `onclick="toggleMenu()"`: Calls a JavaScript function to toggle the menu on mobile devices.

---

### **Background & Styling**
```html
<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
- Resets default margins and paddings.

```html
body {
    background-color: #D2D2D2;
    background-image:
    repeating-linear-gradient(
        to right, transparent 0 100px,
        #25283b22 100px 101px
    ),
    repeating-linear-gradient(
        to bottom, transparent 0 100px,
        #25283b22 100px 101px
    );
}
```
- Sets a **gray background** with **grid-like patterns**.

```html
body::before {
    position: absolute;
    width: min(1400px, 90vw);
    top: 10%;
    left: 50%;
    height: 90%;
    transform: translateX(-50%);
    content: '';
    background-image: url(2.jpg);
    background-size: 100%;
    background-repeat: no-repeat;
    background-position: top center;
    pointer-events: none;
}
```
- Displays an **overlay image (`2.jpg`)** centered on the page.

---

### **Slider (Banner with Images)**
```html
<div class="banner">
    <div class="slider" style="--quantity: 10">
```
- `<div class="banner">`: Container for the slider.
- `<div class="slider">`: Holds multiple images for the slider.

#### **Slider Images**
```html
    <div class="item" style="--position: 1"><img src="to.jpg" alt=""></div>
    <div class="item" style="--position: 2"><img src="t1.jpg" alt=""></div>
    <div class="item" style="--position: 3"><img src="t4.png" alt=""></div>
```
- Each `<div class="item">` holds an `<img>`.

```html
    <div class="middle-image">
        <img src="takshashila.webp" alt="Takshashila">
    </div>
```
- **Adds a special image (Takshashila University) in the center.**

---

### **Dark Reality Section**
```html
<section class="dark-reality">
    <h2 class="fade-in">The System That Created Slaves</h2>
```
- `<section>`: Defines a webpage section.
- `<h2>`: Section title.

```html
    <div class="grid">
        <div class="item">
            <img src="dr1.jpeg" alt="Factory-like education">
            <p>From Gurukuls to factories – minds trained to obey, not to think.</p>
        </div>
```
- **Shows how education changed from Gurukul systems to rote learning.**

---

### **Lost Knowledge Section**
```html
<section class="lost-knowledge">
    <h2 class="slide-up">What We Lost</h2>
```
- Section **title**.

```html
    <div class="card">
        <img src="lt-1.jpeg" alt="Takshashila University">
        <p>The first global university, where 10,000+ students studied.</p>
    </div>
```
- **Mentions lost ancient educational institutions.**

---

### **Revival Section**
```html
<section class="revival">
    <h2 class="neon-glow">Rebuilding Our Legacy</h2>
```
- Section **title with neon glow effect.**

#### **Courses**
```html
<div class="course">
    <img src="rb-1.jpeg" alt="AI in Ancient India">
    <p>AI before its time – hidden knowledge decoded.</p>
    <button>Learn More</button>
</div>
```
- **Each `div.course` highlights a topic (AI, Quantum Computing, Cybersecurity).**
- **Button changes color on hover.**

---

### **Footer Section**
```html
<footer>
    <div class="footer-container">
```
- **Creates a footer for the page.**

#### **Footer Left**
```html
<div class="footer-left">
    <h3>Sanatana Awakening</h3>
    <p>Empowering minds with lost wisdom and modern intelligence.</p>
</div>
```
- **Website branding.**

#### **Footer Center (Quick Links)**
```html
<ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Courses</a></li>
    <li><a href="#">Books</a></li>
</ul>
```
- **Quick navigation links.**

#### **Footer Right (Social Media)**
```html
<div class="social-icons">
    <a href="#"><i class="fab fa-facebook"></i></a>
    <a href="#"><i class="fab fa-instagram"></i></a>
    <a href="#"><i class="fab fa-twitter"></i></a>
</div>
```
- **Social media icons.**
------

# **📌 Full Breakdown of  CSS**
## **1️⃣ General Page Styling**
```css
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: rgb(0, 0, 0);
    color: rgb(239, 235, 235);
}
```
### **What this does:**
- **`margin: 0;`**  
  - Removes the default margin around the page.
- **`font-family: Arial, sans-serif;`**  
  - Sets the text to use **Arial** first. If Arial isn’t available, it falls back to any **sans-serif** font.
- **`background: rgb(0, 0, 0);`**  
  - Sets the **background color** to **black**.
- **`color: rgb(239, 235, 235);`**  
  - Sets the **text color** to a **light grayish-white**, making it readable against the dark background.

---
## **2️⃣ Navbar (Navigation Bar)**
```css
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: rgba(240, 209, 209, 0.1);
    padding: 15px 50px;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}
```
### **What this does:**
- **`display: flex;`**  
  - Makes the navbar a **flex container**, so items (like links and buttons) align in a row.
- **`justify-content: space-between;`**  
  - Positions items **at both ends** of the navbar (logo on the left, links on the right).
- **`align-items: center;`**  
  - Vertically centers the navbar items.
- **`background: rgba(240, 209, 209, 0.1);`**  
  - Makes the navbar **slightly transparent**.
- **`padding: 15px 50px;`**  
  - Adds **top/bottom (15px)** and **left/right (50px)** spacing.
- **`position: fixed;`**  
  - Fixes the navbar **at the top** of the screen, so it doesn’t scroll away.
- **`width: 100%;`**  
  - Makes the navbar stretch across the entire width.
- **`top: 0;`**  
  - Ensures the navbar stays at the **very top**.
- **`z-index: 1000;`**  
  - Ensures the navbar **stays above** all other elements.

---
## **3️⃣ Navbar Links**
```css
.nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
}
```
### **What this does:**
- **`list-style: none;`**  
  - Removes **default list bullets**.
- **`display: flex;`**  
  - Makes the links **align in a row**.
- **`gap: 20px;`**  
  - Adds **spacing between links**.

```css
.nav-links a {
    color: rgb(230, 65, 6);
    text-decoration: none;
    font-size: 18px;
    padding: 10px;
    transition: 0.3s;
}
```
### **What this does:**
- **`color: rgb(230, 65, 6);`**  
  - Makes the links **orange-red**.
- **`text-decoration: none;`**  
  - Removes the **default underline** from links.
- **`font-size: 18px;`**  
  - Sets the **font size**.
- **`padding: 10px;`**  
  - Adds space around the links.
- **`transition: 0.3s;`**  
  - Creates a **smooth hover effect**.

---
## **4️⃣ Hover Effects for Links**
```css
.nav-links a:hover {
    color: rgb(243, 128, 28);
    background: rgba(255, 255, 255, 0.2);
    border-radius: 5px;
}
```
### **What this does:**
- **Changes color to a lighter orange when hovered**.
- **Adds a semi-transparent background**.
- **Rounds the corners slightly**.

---
## **5️⃣ Navbar Buttons**
```css
.nav-buttons {
    display: flex;
    gap: 10px;
}
```
### **What this does:**
- **`display: flex;`**  
  - Aligns buttons in a row.
- **`gap: 10px;`**  
  - Adds **space between buttons**.

```css
.btn {
    padding: 8px 16px;
    border-radius: 5px;
    font-size: 16px;
    text-decoration: none;
    transition: 0.3s;
}
```
### **What this does:**
- **Creates a common button style**.
- **Smooth hover effect**.

---
## **6️⃣ Login and Signup Buttons**
```css
.btn.login {
    background: transparent;
    border: 2px solid rgb(245, 116, 51);
    color: rgb(249, 187, 64);
}
```
### **What this does:**
- **Transparent background**.
- **Orange border**.
- **Golden yellow text**.

```css
.btn.login:hover {
    background: rgb(241, 139, 37);
    color: black;
}
```
### **What this does:**
- **Turns background orange and text black on hover**.

---
## **7️⃣ Signup Button**
```css
.btn.signup {
    background: rgb(249, 112, 33);
    color: black;
    border: 2px solid rgb(251, 187, 49);
}
```
- **Orange background with a lighter orange border**.

```css
.btn.signup:hover {
    background: rgb(0, 0, 0);
    color: black;
}
```
⚠ **Problem:** The text also turns **black**, making it invisible.

---
## **8️⃣ Mobile Responsive Navbar**
```css
@media (max-width: 768px) {
    .nav-links {
        display: none;
        flex-direction: column;
        position: absolute;
        background: black;
        width: 100%;
        top: 60px;
        left: 0;
        padding: 10px;
    }

    .nav-links.active {
        display: flex;
    }

    .hamburger {
        display: block;
        font-size: 28px;
        color: white;
        cursor: pointer;
    }
}
```
### **What this does:**
- **Hides navbar links on small screens**.
- **Adds a hamburger menu**.
- **Displays links when clicked**.

---
## **9️⃣ 3D Slider**
```css
@keyframes autoRun {
    from {
        transform: perspective(1200px) rotateX(-16deg) rotateY(0deg);
    }
    to {
        transform: perspective(1200px) rotateX(-16deg) rotateY(360deg);
    }
}
```
### **What this does:**
- **Creates a 3D spinning effect**.

---
## **🔟 Section Titles with Flickering Effect**
```css
.dark-reality h2 {
    text-transform: uppercase;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(45deg, #ff0000, #8b0000);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    letter-spacing: 3px;
    animation: flicker 1.5s infinite alternate;
}
```
### **What this does:**
- **Red gradient text**.
- **Creates a flickering effect**.

---

## **1. Importing Fonts**  

```css
@import url('https://fonts.cdnfonts.com/css/old-english-five');
@import url('https://fonts.cdnfonts.com/css/poppins');
```
- This imports **two custom fonts** from an external font CDN (Content Delivery Network).
- **`Old English Five`** is likely used for titles or headings.
- **`Poppins`** is a clean, modern sans-serif font for body text.

---

## **2. Body Styling**  

```css
body {
    background: linear-gradient(to bottom, #2c1d0f, #000000, #000000);
    font-family: 'Poppins', sans-serif;
    color: #faf7f7;
    margin: 0;
    overflow-x: hidden;
}
```
### **Explanation:**
1. **`background: linear-gradient(to bottom, #2c1d0f, #000000, #000000);`**
   - Creates a **gradient background** from **dark brown (#2c1d0f) at the top** to **black (#000000) at the bottom**.
   
2. **`font-family: 'Poppins', sans-serif;`**
   - Sets the default **font** for the page to **Poppins**.

3. **`color: #faf7f7;`**
   - Sets the **text color** to **light grayish-white (#faf7f7)**.

4. **`margin: 0;`**
   - Removes any **default margin** around the body.

5. **`overflow-x: hidden;`**
   - Prevents **horizontal scrolling**, ensuring content does not overflow the viewport.

---

## **3. Overwriting Background Color**  

```css
body {
    background: black !important;
}
```
- This **forces** the background to **black** using `!important`, overriding any previous background styles.

---

## **4. Banner & Slider Styling**  

```css
.banner {
    background: black !important;
}
```
- **Forces** the banner’s background to be **black** using `!important`.

```css
.slider {
    background: transparent;
}
```
- Makes the **slider background transparent**.

```css
.slider img {
    width: 100%;
    height: 100%;
    object-fit: contain;
}
```
### **Explanation:**
1. **`width: 100%;`** → Ensures the image stretches **full width** of its container.
2. **`height: 100%;`** → Ensures it takes the **full height** of its container.
3. **`object-fit: contain;`** → Ensures the **entire image is visible** inside the container **without cropping**.

---

## **5. Banner Slider Item Shadow**
```css
.banner .slider .item {
    box-shadow: 0px 10px 20px rgba(255, 204, 0, 0.5);
}
```
- Adds a **shadow** to slider items:
  - **`0px`** → No horizontal shadow.
  - **`10px`** → Moves shadow **down by 10px**.
  - **`20px`** → Blurs the shadow.
  - **`rgba(255, 204, 0, 0.5)`** → **Yellow-orange shadow (50% opacity).**

---

## **6. 3D Slider Setup**
```css
.banner {
    width: 100%;
    height: 100vh;
    text-align: center;
    overflow: hidden;
    position: relative;
}
```
### **Explanation:**
1. **`width: 100%;`** → Makes the banner **full width**.
2. **`height: 100vh;`** → Takes **full viewport height**.
3. **`text-align: center;`** → Centers the text **inside the banner**.
4. **`overflow: hidden;`** → Hides any overflowing content.
5. **`position: relative;`** → Allows absolute-positioned child elements to be placed relative to the banner.

```css
.banner .slider {
    position: absolute;
    width: 220px;
    height: 300px;
    top: 12%;
    left: calc(50% - 110px);
    transform-style: preserve-3d;
    transform: perspective(1000px);
    animation: autoRun 18s linear infinite;
    z-index: 2;
}
```
### **Explanation:**
1. **`position: absolute;`** → Positions the slider **inside the banner**.
2. **`width: 220px;`** → Sets **width of the slider**.
3. **`height: 300px;`** → Sets **height of the slider**.
4. **`top: 12%;`** → Moves it **down 12% from the top**.
5. **`left: calc(50% - 110px);`** → Centers the slider.
6. **`transform-style: preserve-3d;`** → Enables **3D transformations**.
7. **`transform: perspective(1000px);`** → Adds **depth perspective** (like looking into a cube).
8. **`animation: autoRun 18s linear infinite;`** → Rotates the slider automatically.

---

## **7. 3D Rotation Animation**
```css
@keyframes autoRun {
    from {
        transform: perspective(1200px) rotateX(-16deg) rotateY(0deg);
    }
    to {
        transform: perspective(1200px) rotateX(-16deg) rotateY(360deg);
    }
}
```
- **Creates a rotating effect** for the slider:
  - **Starts from** `rotateY(0deg)`.
  - **Ends at** `rotateY(360deg)`, making a **full spin**.

---

## **8. Ensuring Navbar Visibility**
```css
.slider {
    z-index: 1;
}
.navbar {
    z-index: 10;
}
```
- **Ensures** the `navbar` appears **above the slider**.

---
---

### **9.3d images**
```css
.banner .slider .item {
    position: absolute;
    inset: 0 0 0 0;
    transform: rotateY(calc((var(--position) - 1) * (360 / var(--quantity)) * 1deg)) translateZ(600px);
}
```
#### **Explanation:**
- **`position: absolute;`**  
  - The `.item` (book cover) is positioned absolutely relative to its parent `.slider`.  
  - This means it is removed from the normal document flow and positioned based on the nearest positioned ancestor.
  
- **`inset: 0 0 0 0;`**  
  - This is shorthand for `top: 0; right: 0; bottom: 0; left: 0;`.  
  - It makes sure the `.item` element stretches across the entire `.slider` container.  

- **`transform: rotateY(calc((var(--position) - 1) * (360 / var(--quantity)) * 1deg)) translateZ(600px);`**  
  - **`rotateY(calc((var(--position) - 1) * (360 / var(--quantity)) * 1deg))`**  
    - Rotates each book cover along the Y-axis by a specific angle.  
    - The angle is calculated dynamically based on the `--position` and `--quantity` of items in the slider.  
    - This ensures a circular 3D arrangement.  
  - **`translateZ(600px);`**  
    - Moves the book cover forward along the Z-axis, making it appear in 3D space.  
    - A higher value moves it further out of the screen.

---

### **10. Glowing Hover Effect**
```css
.banner .slider .item:hover {
    transform: scale(1.1) rotateY(calc((var(--position) - 1) * (360 / var(--quantity)) * 1deg)) translateZ(620px);
    box-shadow: 0px 0px 25px rgba(255, 204, 0, 0.8);
}
```
#### **Explanation:**
- **`transform: scale(1.1)`**  
  - Increases the size of the item by **10%** when hovered.  
  - This gives a zoom effect.  

- **`rotateY(calc((var(--position) - 1) * (360 / var(--quantity)) * 1deg))`**  
  - Keeps the original Y-axis rotation intact so the book remains in the circular arrangement.  

- **`translateZ(620px);`**  
  - Moves the item slightly **forward (by 20px more than normal)** to make it stand out when hovered.  

- **`box-shadow: 0px 0px 25px rgba(255, 204, 0, 0.8);`**  
  - Adds a **glowing effect** around the book.  
  - **`rgba(255, 204, 0, 0.8);`** represents a **yellow glow** (RGB: 255, 204, 0) with 80% opacity.  

---

### **11. Titles & Fonts**
```css
.banner .content h1 {
    font-family: 'Old English Five', serif;
    font-size: 5em;
    color: #f32613;
}
```
#### **Explanation:**
- **`font-family: 'Old English Five', serif;`**  
  - Uses a **Gothic-style font** for the title.  
  - The **fallback font** is a generic **serif** font.  

- **`font-size: 5em;`**  
  - Makes the font **very large** (5 times the default text size).  

- **`color: #f32613;`**  
  - Sets the text color to a **bright red shade** (`#f32613`).  
### **Detailed Explanation of the CSS Code**

---

### **1. Middle Image Styling**
```css
.middle-image {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 100;
}
```
- **`position: absolute;`** → Positions the element relative to its nearest positioned ancestor.
- **`top: 50%; left: 50%;`** → Moves the element to the center of the screen.
- **`transform: translate(-50%, -50%);`** → Adjusts the element to be perfectly centered.
- **`z-index: 100;`** → Ensures the image appears above other elements.

```css
.middle-image img {
    width: 600px; /* Increase size */
    height: auto;
    border: 3px solid white; /* Optional border */
    box-shadow: 0px 0px 15px rgba(255, 255, 255, 0.7);
    transform: scale(1.3); /* Slight zoom effect */
}
```
- **`width: 600px;`** → Enlarges the image.
- **`height: auto;`** → Maintains the aspect ratio.
- **`border: 3px solid white;`** → Adds a white border.
- **`box-shadow: 0px 0px 15px rgba(255, 255, 255, 0.7);`** → Creates a glowing effect.
- **`transform: scale(1.3);`** → Slightly enlarges the image.

---

### **2. Section Styling**
```css
section {
    padding: 60px 10%;
    text-align: center;
    background-color: #000;
    color: #fff;
}
```
- **`padding: 60px 10%;`** → Adds space around the content.
- **`text-align: center;`** → Centers text inside the section.
- **`background-color: #000;`** → Black background.
- **`color: #fff;`** → White text for contrast.

---

### **3. Dark Reality Section**
#### **Title Styling**
```css
.dark-reality h2 {
    text-transform: uppercase;
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(45deg, #ff0000, #8b0000);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    letter-spacing: 3px;
    animation: flicker 1.5s infinite alternate;
}
```
- **`text-transform: uppercase;`** → Converts text to uppercase.
- **`font-size: 2.5rem;`** → Large text.
- **`font-weight: 800;`** → Makes the text bold.
- **`background: linear-gradient(45deg, #ff0000, #8b0000);`** → Creates a red gradient text effect.
- **`-webkit-background-clip: text; -webkit-text-fill-color: transparent;`** → Applies gradient only to the text.
- **`letter-spacing: 3px;`** → Increases spacing between letters.
- **`animation: flicker 1.5s infinite alternate;`** → Applies a flickering effect.

#### **Flicker Animation**
```css
@keyframes flicker {
    0% { opacity: 1; }
    50% { opacity: 0.8; }
    100% { opacity: 1; }
}
```
- **Creates a flickering effect by changing opacity.**

#### **Grid Layout for Items**
```css
.dark-reality .grid {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}
```
- **`display: flex;`** → Aligns items in a row.
- **`justify-content: center;`** → Centers items horizontally.
- **`gap: 20px;`** → Adds space between items.
- **`flex-wrap: wrap;`** → Ensures items wrap on smaller screens.

#### **Item Styling**
```css
.dark-reality .item {
    background: #111;
    padding: 20px;
    border-radius: 10px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.dark-reality .item:hover {
    transform: scale(1.05);
    box-shadow: 0 0 10px #ff7300;
}
```
- **Adds a dark box with rounded corners and hover effects.**
- **On hover:** Slightly enlarges (`scale(1.05)`) and adds an orange glow.

---

### **4. Lost Knowledge Section**
#### **Title Styling**
```css
.lost-knowledge h2 {
    font-size: 2.8rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: #ff9f1c;
    text-shadow: 2px 2px 10px rgba(255, 159, 28, 0.7);
    transition: all 0.3s ease-in-out;
}

.lost-knowledge h2:hover {
    color: #ff5400;
    transform: scale(1.05);
}
```
- **Uses a golden-orange theme with text-shadow for glow.**
- **On hover:** Changes color and slightly enlarges the title.

#### **Card Layout**
```css
.lost-knowledge .flex-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}
```
- **Same flex properties as `.dark-reality .grid` for responsiveness.**

#### **Card Styling**
```css
.lost-knowledge .card {
    background: #111;
    padding: 20px;
    border-radius: 10px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.lost-knowledge .card:hover {
    transform: scale(1.05);
    box-shadow: 0 0 10px #ff7300;
}
```
- **Adds a dark card with hover effects.**

---

### **5. Revival Section**
#### **Title Styling**
```css
.revival h2 {
    font-size: 3rem;
    font-weight: 900;
    text-transform: uppercase;
    background: linear-gradient(45deg, #ff7300, #ffcc00);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    letter-spacing: 4px;
    text-shadow: 3px 3px 15px rgba(255, 204, 0, 0.5);
    animation: glow 2s infinite alternate;
}
```
- **Gradient text with animation.**
Glow Animation:
css
Copy
Edit
@keyframes glow {
    0% { text-shadow: 3px 3px 15px rgba(255, 204, 0, 0.5); }
    100% { text-shadow: 5px 5px 25px rgba(255, 204, 0, 0.9); }
}
Increases glow intensity over time.
Carousel Layout:
css
Copy
Edit
.revival .carousel {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}
Aligns courses in a horizontal carousel-like format.
Course Styling:
css
Copy
Edit
.revival .course {
    background: #111;
    padding: 20px;
    border-radius: 10px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.revival .course:hover {
    transform: scale(1.05);
    box-shadow: 0 0 15px #ff7300;
}
Hover effect is similar to .card but with a stronger glow.
6. Responsive Design
General Adjustments:
css
Copy
Edit
@media screen and (max-width: 1023px) {
    .banner .slider {
        width: 180px;
        height: 250px;
        left: calc(50% - 90px);
    }
}
@media (max-width: 768px) {
    .history-card {
        padding: 15px;
    }
}
Adjusts .slider size for smaller screens.
Reduces padding for .history-card.
