## REPORTS (Accessibility report (4))

- Interactive controls must not be nested
```html
<button class="btn"><a href="https://github.com/Iron-Mark" target="_blank" rel="noferrer noopener">Learn More</a></button>
```

- Page should contain a level-one heading
```html
<html lang="en">
```

- Bad value "noferrer noopener" for attribute "rel" on element "a": The string "noferrer" is not a registered keyword.
- The element "a" must not appear as a descendant of the "button" element.
```html
<button class="btn">
  <a href="https://github.com/Iron-Mark" target="_blank" rel="noferrer noopener">`
</button>
```

## Community Feedback: 
- __Kamil__ • 90 [_(@Owczarek-Kamil)_](https://github.com/Owczarek-Kamil)
  - You should **not nest buttons** and **`<a>` tags together**
    - This also have been pointed out in the FrondEndMentor Accessibility report and HTML validation report.
    - In my opinion you should <u>go with `<a>` tags and style them with pseudo classes like, :link, :active, :hover, :visited.</u>
  - You should put 'alt' on the icons. But **if the icons do not represent any UX purpose/their purpose is decorative one.**
    - `alt` should be left blank, 
    - And you should include aria-hidden="true".
  - **Implement some hover animations** on buttons/links.
    - Right now the transition is instant and it is not very pleasing for the eyes :)
    - Simple `transition: all 300ms;` would do the work.

<br>

- __バレンタイン 😈__ • 61,400 [_(@Valentine-D3V)_](https://github.com/Valentine-D3V)
  - DO NOT FORGET to **check your FEM report** (It provides value information), 
    - To see what is incorrect and update your code with it. 
    - This should be done immediately after submitting your challenge.
  - **The `section` element is being used incorrectly** and not needed for this challenge.
    - You are using it to wrap each individual card in a section element instead of using a div.
    - The section element is meant group related content in full sites. They are not meant to contain small things like you did.
    - If this was part of a real site, the entire thing would be wrapped in a section and it will have an h2 heading saying something like "Check out our models..."
  - The “car icons” in this component are purely decorative. 
    - **Their `alt` tag should be left blank** to <u>remove them from assistive technology</u>.
  - **`buttons` were created with the incorrect element**
    - When the user clicks on the button they should be directed to a different part of you site. 
    - The anchor tag will achieve this.
  - There is **no need to have separate stylesheets**. Instead have one single stylesheet.
    - As it can affect site performance.


## Next Action (Soon):
- I'm going to review other people's code and how it was done.
- Learn from it and combine it with the suggestions
- Then re-create the website project.