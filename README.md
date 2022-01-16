Day1:
1. Avoid setting a height to anything in css.
2. When you set widths, they are in relation to their parent.
3. Use percentages for widths
4. Webpages are responsive by default. It is us that makes them unresponsive with our poor css
5. box-sizing: border-box; when you add padding and border to a div, it increases the width and size of the div. By setting box-sizing: border-box, the max size of the box shrinks down to accomidate any border and padding. By doing this we can set divs to be 100% width and not have them overflow

Day2:
1. em means that the value (typially fonts) is in relation to their parent element. So a parent with 16px font and a child with 1em will be 16px. if 2em then 32px.
2. A problem with ems is it cascades, and if you keep adding parents or new divs then it may chain down and cause problems.
3. Rems were invented to fix this compounding problem. Rem stands for 'root em'
4. Rem looks at the root parent, which is usually html {}
5. if you use em on margin, it is looking at the font size of it's own div, not the parent
6. Rems ALWAYS look at the root.
7. Better to have rems for stuff like margin, because it will be consistent. If you use em it will vary between divs because it's based off of their individual font sizes
8. Use rem for font. set ::root {} or just use html{}
9. ems are better for margin and padding because they reference that element not the parent
10. max-width is good, min-width not really