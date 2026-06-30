# Classic  Cheese Omelette — Recipe Page

A clean, responsive recipe page built from scratch with semantic HTML and modern CSS. No frameworks, no shortcuts  just structured markup and intentional styling, built to look like something you'd actually find on a real food blog.

## About This Project

This started as a simple HTML/CSS exercise and turned into a deeper dive into what actually makes a webpage feel "designed" rather than just thrown together. The goal was to take a basic recipe layout and push it toward something polished: proper visual hierarchy, breathing room between sections, and a color palette that actually fits the dish instead of defaulting to whatever looked fine at the time.

## What It Includes

The page is built around a single recipe card containing an image, a short description, a preparation time summary, an ingredients list, step-by-step instructions, and a nutrition table. It's wrapped in a proper site header with breadcrumb navigation and a footer, so it reads less like an isolated snippet and more like a real page from a working site.

## Built With

- HTML5, written with semantic tags throughout
- CSS3, including Flexbox and CSS Grid
- Google Fonts (Playfair Display for headings, Inter for body text)

## Technical Highlights

**Layout**
Flexbox handles the horizontal rows — the prep/cook/total time summary  both rely on it to stay aligned and responsive. CSS Grid handles the ingredients list, splitting it into two columns on larger screens and collapsing to one on mobile.

**Semantic structure**
Every element is chosen for what it actually represents, not just how it looks. Ingredients live in a `ul` since order doesn't matter. Instructions live in an `ol` since it does. Nutrition facts live in a proper `table` with `thead` and `tbody`, instead of being faked with divs. The page also uses `header`, `main`, `article`, `section`, and `footer` instead of leaning on generic divs everywhere.



**Styling**
All CSS lives in a single external stylesheet — there isn't a single inline style anywhere in the HTML. Visual hierarchy comes from font size, weight, and color rather than just bigger text. Earthy, warm tones were chosen to match the dish itself.

## File Structure

```
index.html
style.css
images/
  IMG_7807.JPG
```

## What I Learned

Going into this, I figured CSS was mostly about making things "look nice." What actually slowed me down and taught me the most  was realizing how much of good design is really about restraint and structure, not decoration.

Getting the ingredients list into a clean two-column grid was the first real "click" moment with CSS Grid. I'd used Flexbox a fair amount before, but Grid forced me to think differently less about pushing items around in a line and more about defining the shape of the layout up front.

Switching the nutrition section from a list to an actual `table` also changed how I think about HTML in general. It would've been easier to keep using divs and style them to look table-like, but that's not what they are. Using the right tag for the right job made the markup easier to read and, more importantly, made it actually accessible to screen readers without extra work.

Spacing was the most underrated lesson. Early versions of this page felt cramped even though the content itself wasn't wrong it just needed more margin and padding between sections to breathe. A few pixels of consistent spacing did more for the "professional" feel than any color or font choice did.


Lastly, working in small, testable sections — info row, then ingredients, then instructions, then nutrition — made the whole project far less overwhelming than trying to style the entire page at once. Breaking things down made debugging faster and kept me from losing track of what I'd already finished.

