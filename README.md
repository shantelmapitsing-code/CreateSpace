# CreateSpace - Youth Creative Hub

Student: Shantel Malihu Mapitsing
Module code: WEDE5020
File: css_assets/myfirststyles.css (Single CSS File)

## Project Overview
CreateSpace was established in 2022 as a community-based organisation that helps young people explore creative activities and digital skills. It offers workshops in art, photography, film, music, web development, game design and performing arts.


## Design Theme & Decisions

### 5. Design
Colours: 
1.Purple - #7c3aed - Top nav CreateSpace header
2.Pink - #ec4899 - Join button + EST tag
3.Blue - #3b82f6 – Headings
4.Light Purple joining - #e9d5ff - 4px line under header
5.Off-white - #f8f5ff - inner background


### 2.2 Typography
font-family:'Poppins', sans-serif; /* font-family */
  font-size:1rem; /* font-size rem */
  font-weight:400; /* font-weight */
  line-height:1.7; /* line-height */
  letter-spacing:0.02em; /* letter-spacing */
  color:lch(29.13% 115.08 306.37); /* color */
  background:rgb(255, 192, 238); 

### 2.3 Layout System
1. Header → Navigation → Content → Footer.
2. Flexbox : .site-header uses display:flex, flex-direction:row, justify-content:space-between, align-items:center
3. Grid : .hero-section uses display:grid, grid-template-areas:"content visual", grid-template-columns:1fr 1fr
4. No floats, no absolute positioning for main layout


## 3. Technical Implementation
1.	HTML5: Structure - Using semantic tags header, nav, main, section, footer
2.	CSS: Design - External stylesheet css/style.css with Flexbox and Grid
3.	JavaScript: Interaction - Form validation for email and SA phone format, mobile menu toggle, opening hours status using Date() object
4.	Images: Visuals - Optimized WebP under 200KB with alt text
5.	Responsive design: All devices - Breakpoints 375px mobile, 768px tablet, 1024px desktop
6.	Domain: http://brightfuturelibrary.co.za - Available at http://Domains.co.za (2026), Hosting at xneelo (2026).


### 3.2 Relative Units
All layout uses relative: em, %, rem, 100% - No px for width/padding/margin except border-radius/shadow which is allowed.
Examples: padding:1em 5%, width:96%, font-size:1rem, max-width:100%


### 3.3 Visual Effects
1) background: hwb(293 23% 7%);
   border-bottom:4px solid #ec4899;
   box-shadow:0 4px 15px rgba(0,0,0,0.15);

2) .main-menu a:hover { background:#fff; color:#7c3aed; } /* HOVER */

3)  a:focus { outline:2px solid #fff; }
    a:active { background:#ec4899; }


### 3.4 Images 
img { max-width:100%; display:block; border-radius:12px; }
.hero-visual img { width:100%; max-width:380px; height:320px; max-height:320px; object-fit:cover; }
.content-card img { width:100%; height:150px; max-height:150px; object-fit:cover; border-radius:10px; margin-bottom:1em; }


## 4. Responsivenes
- Desktop: card-grid = 3 columns
- 768px breakpoint: card-grid = 2 columns, header stacks
- 480px breakpoint: card-grid = 1 column, menu full width

## Visual Effect
- Cards have `border-top:4px solid` with different colors + `box-shadow`
- Hover: `transform:translateY(-5px)` lift effect


## 5. Testing & Validation 

### 5.1 Before/After Bug
**Before:** Images 800px huge + RGB duplication glitch (see wa_image_3315589367890985783 original)
**Cause:** No max-height, no object-fit, multiple backgrounds overlapping
**Fix:** Added height:150px; max-height:150px; object-fit:cover; border:4px solid #e9d5ff; to control images and join sections
**After:** Screenshot attached - clean cards, controlled images, purple header consistent

### 5.2 Validation
- W3C CSS Validator: Pass 0 errors
- W3C HTML Validator: Pass 0 errors
- Accessibility: Tab navigation tested, focus visible

## 6. File Structure
The project uses a single external stylesheet as required for distinction:

- All 5 HTML pages link to `css_assets/myfirststyles.css`
- No inline styles or `<style>` tags used
- Images use `srcset` and `sizes` for responsiveness
- Relative units used throughout (%, em, rem, vw)


## References

Krug, S., 2023. _Don't make Me Think, Revisited: A Common Sense Approach to Web Usability._ 3rd ed. Berkeley: New Riders.
Pexels, 2023. _Pexels License._ Available at: https://www.pexels.com/license/ [Accessed 20 August 2023]. [Online]

Rubin, J. and Chisnell, D., 2022. _Handbook of Usability Testing: How to Plan, Design, and Conduct Effective Tests._ 2nd ed. Indianapolis: Wiley.

W3C, 2023. _W3C Markup Validation Service._ Available at: https://validator.w3.org/ [Accessed 18 August 2023]. [Online]

W3Schools, 2023. _HTML Tutorial._ Available at: https://www.w3schools.com/html/ [Accessed 14 August 2023]. [Online]


