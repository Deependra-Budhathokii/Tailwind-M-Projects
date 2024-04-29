# Responsive Navbar Project:

## ***Building Environement Installation and Setup

In the options of  `Tailwind CLI`, `Using PostCSS` , `Framework Guides`
Lets Install with `Tailwind CLI`



## Project Overview
Briefly describe the purpose and goals of creating the responsive navbar.

## Color Scheme
Outline the color palette for the navbar. Include hex codes for consistency.
- nav menu hover color : `text-gray-500`
- Primary color: `#hexcode`
- Secondary color: `#hexcode`
<!-- - Accent color: `#hexcode` -->

## Typography
Detail the typography choices for the navbar. Include font families, sizes, and any particular styling considerations.
- Font- poppins  (use google fonts)

### Styling Idea and utilities
- utilities class : duration-500
- 


## Tailwind CSS Configuration
Explain any custom configurations you plan to use in Tailwind CSS. This could include:
- Custom utilities
- Responsive breakpoints
- Hover and focus states

## JavaScript Interactions
Describe any JavaScript-driven interactions (e.g., dropdowns, mobile menu toggle). Outline the functions and any libraries or frameworks you plan to use.

## Accessibility Considerations
List the steps you will take to ensure the navbar is accessible. Consider aspects like keyboard navigation and screen reader compatibility.

## Rough Timeline
Provide a basic timeline for the project. Break it down into phases like:
- Research and planning
- Design
- Development
- Testing
- Deployment

## Challenges and Solutions
Identify potential challenges you might face during the development and propose preliminary solutions or resources to tackle these issues.

## References
List any resources, articles, or documentation that will be referenced throughout the project.


## <span style="color:yellow"> Responsive Navbar Section Pre Plan

### Layout Design
- Features used : `Flex`
- Logo image Links : https://cdn-icons-png.flaticon.com/512/5968/5968204.png


For mobile device  Drop down menu:
- height : 60vh
- use positions
- To rectify height 60vh in larger screen use `h-fit`
- To rectify `w-full` in larger screen use `w-auto`

- use `menu icons` - from iconic icons

### js part
use `tooggling the class property logic`
- toggle classList 


### Styling Idea and utilities
- utilities class : duration-500
- btn bg color: bg-[#a6c1ee],  add hover color also

### <span style="color:teal"> Responsive Navbar Section post Review
.....



----------------------------------------------------------
# Responsive Navabar Mini Project    
----------------------------------------------------------

- `left-0` which makes the responsive nav-bar take `full width space` 

- `min-h-[60vh]  md:min-h-fit`     // if we need to give min-h[for small screen] and but in larger screen no height is mentioned we can use `min-h-fit`


- `w-full md:w-auto`   // if we need to provide 100% width to small screen i.e`w-full` and in that case no width is specifically mentioned for larger screen, we can use `w-auto` for larger screen


- `left-0 top-[9%]`, we do not need to rectify this for `larger screen` as this apply only when position is `absolute` but for larger screen, we have make it `md:static` so this positioning will not be applied for `larger screen`

- Now we make `top-[-100%]` // we change value from 9% to -100%, to make it hidded



***using `toggle() method` of the `classList property` For functioning of Menu Buttons*** 

- Basic logic used is we toggle the value between top-[9%] and top-[-100%]

<!-- html part -->
<div class="duration-100 nav-links top-[-100%]">
<nav>li*5</nav>
</div>

<icon name="menu" onClick="onToggleMenu(this)">

<!-- Js part -->

<script>
  const navLinks = document.querySelector('.nav-links')
  navLinks.classlist.toggle('top-[9%]')
</script>


- `duration-1000`  equivalent to transition-durarion:1000s


----------------------------------------------
`Using Display flex for single item`
----------------------------------------------
```
<div class= "flex items-center h-[60vh]">
<div></div>
</div>

```
----------------------------------------------
