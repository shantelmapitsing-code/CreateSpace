# CreateSpace Youth Centre - WEDE5020 Part 2
Student Name: Malihu Shantel Mapitsing
Student Number: st10475897
Module code: WEDE5020

Single Stylesheet: css_assets/myfirststyles.css

## What I Changed From Part 1 (Fixes)

1.  Sitemap: Part 1 was just a plain text list. So I fixed it and added a sitemap
2.  References: Part 1 had only 2 sources with no dates. Fixed to 5 sources with full URLs and Date Accessed
3.  Timeline: Part 1 timeline was 2 lines. Fixed to a full Table with columns: Week | Task | Deliverable | Status (Week 1-8).
4.  Wireframe: Part 1 wireframe was not there. Re-did it as clear hand-drawn + labelled with header, nav, hero, card-grid, footer.
6.  Images: Part 1 images were 3MB and broken. Replaced with resized 480w and 800w versions and deleted corrupted files.
7.  HTML Structure: Fixed all pages to use same header/footer and added alt text to all images. Had to separate all 5 files because they were all under one file which was the index.html
8.  Also added comments on my code they were not there in part1

## What I Added in Part 2 (New for Distinction)

1. Single External CSS:Created `CSS assets/myfirststyles.css` - all 5 pages link to it
2. Visual Effects:
   - Cards: `background:#fff0f6`, `border-top:4px solid #ec4899`, `border-radius:16px`, `box-shadow`
   - Hover: `transform:translateY(-5px)` + deeper shadow
   - 3 different colors for 3 cards (pink #ec4899, purple #7c3aed, blue #3b82f6)

3. Responsiveness :
   - Relative units: Used %, em, rem, vw, vh throughout (no px for layout)
   - Media Queries: `@media max-width:768px` and `480px`
   - Tablet: header flex-direction:column, card-grid 1fr 1fr
   - Mobile: card-grid 1fr, menu 100% width

4. Responsive Images:
   - Used `<picture>` + `srcset` + `sizes` attributes
   - Example: `srcset="photography-480.jpg 480w, photography-800.jpg 800w"`
   - `sizes="(max-width:480px) 90vw, (max-width:768px) 80vw, 400px"`
   - CSS: `max-width:100%`, `height:auto`, `object-fit:cover`

## File Structure
- All HTML files are in root for easy linking
- `css_assets/` contains only 1 CSS file as required for distinction
- `images/` contains responsive versions (480w and 800w) to fix broken rainbow images from Part 1
- `proposal/` contains updated Part 1 documents

  ### References
Krug, S., 2023. _Don't make Me Think, Revisited: A Common Sense Approach to Web Usability._ 3rd ed. Berkeley: New Riders.

W3C, 2023. _W3C Markup Validation Service._ Available at: https://validator.w3.org/ [Accessed 18 August 2023]. [Online]

W3Schools, 2023. _HTML Tutorial._ Available at: https://www.w3schools.com/html/ [Accessed 14 August 2023]. [Online]

Pexels, 2023. _Pexels License._ Available at: https://www.pexels.com/license/ [Accessed 20 August 2023]. [Online]

Rubin, J. and Chisnell, D., 2022. _Handbook of Usability Testing: How to Plan, Design, and Conduct Effective Tests._ 2nd ed. Indianapolis: Wiley.
