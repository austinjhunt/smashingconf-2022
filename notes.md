# Smashing Conference 2022
#smashingconf
## Conference Day 1
smashed.by/rock
### Brad Frost - Creating Themable Design System
A design system is like **wellness** in a post-covid world.
- important
- no one has it
- we pretend like we have it when talking with others
- companies pretend to care about it
- achieving it harder han it sounds
- desperately need more time and resources to work on it

- What's a design system?
  - the story of how your organization designs and builds digital interfaces
- Buttons
  - inventory, lots of time & money & meetings, even just for buttons
- Themeability allows for significant reuse. Keep your same set of components, change the skeletal structure of all of them by changing the theme. Same markup, different look and feel with each theme. 

- Themeable Design Systems can support
  - multiple brands
  - sub-brands
  - white-labeling
  - multiple generations of a design language
  - multiple platforms or product families (web app vs marketing website)
  - seasons, campaigns
  - dark mode, light mode

- How do you do it?
  - CSS is most malleable layer of stack. Want rock-solid HTML, JS. Then use CSS to flow different things through it. 
  - Don't hardcode styles into components. Use **design tokens**
- Design Tokens
  - subatomic particles of our interfaces
  - implementation-agnostic source of truth
  - properties
    - colors
    - font sizes
    - font weights
    - line heights
    - border thicknesses
    - border radii
    - animation vars
    - breakpoints
    - spacing
    - type colors
    - background colors
^^^^
Communications <-> native apps <-> marketing site <-> product 1 <-> product 2
  - 3-tiered Token System
    - Tier 1 Tokens: Definitions
      - just identify all of your raw ingredients, like dumping ikea parts out on the table
      - with typography, instead of just one value that travels together, group together font family, font weight, font size, and line height into a typography preset, don't split them up 
    - Tier 2 Tokens: 
      - Semantic usage
        - theme-color-background-brand: < one of those defined raw ingredients that can be switched out for another value >
      - Semantic Typography
    - Tier 3: Design System Components Variables
      - e.g. class-name : theme-color-background-brand
  - Theme Layer
    - Tier 1: Definitions 
    - Tier 2: Theme
  - Tier 3: Component (Design system component library)
  - Component library stays stable
- Figma 
- Theemo - Style Automator, figma does not have this built in; this allows you to create semantic values for things like color
- Themer; allows you to switch between those token sets
- github.com/salesforce-ux/theo
- amzn.github.io/style-dictionary (build system that allows you to define styles once, in a format-agnostic way)
- [Storybook demo](https://storybook.js.org)
- [CSS Zen Garden](http://www.csszengarden.com)
- TL;DR Design Systems + CSS Zen Garden = Awesome
- https://bradfrost.com/blog/post/creating-themeable-design-systems
- [https://github.com/sturobson/Awesome-Design-Tokens](https://github.com/sturobson/Awesome-Design-Tokens)


### Kate Kalcevich - Scaling Up Accessibility
- Accessibility at scale harder than individual / small scale 
- You can 
- Hard ways to achieve accessibility
  - Get sued, complaints, reputation loss, not efficient
  - Build with accessibility in mind; people still complain. Just following guideline not enough, need to test with users who have disabilities. 
- Even if you do rebuild your site piece by piece to make more accessible, will become inaccessible again. Need to have something continuous in place. 
- How do you scale accessibility across an organization?
  - Create a practice of inclusion within your organization.
  - Accessibility needs to fit into all processes; planning, researching, customer service, development
  - Organizations need to start bringing accessibility testing tools into product development lifecycle
  - The point of accessibility is to make something that is usable by everyone including those with disabilities, so people with disabilities need to be involved in the product development lifecycle. UX requires user involvement; Accessibility requires disabled users' involvement.
  - Need user stories geared toward accessibility. E.g. As a partially blind person, I want high contrast text so I can read the information on the website.
  - Accessibility is a team sport.
  - If anyone is not supporting accessibility, you'll have a gap in the end result of your product/website.
- Generative research: learn about peoples' needs, including those with disabilities who depend on assistive technologies
  - Ask about interaction with assistive technology
  - Ask about any specific challenges they might have
  - Before you design product, you should know what the user needs are
  - Ask about any good accessible experiences they've had
- Sheetal - screen magnification user, demo of generative research
- There are accessibility consulting companies that will do consulting for you; lighthouse for the blind
-  Accessibility easier to address in the early planning & research phase than later. 
-  Accessibilty annotations should be added into the design system, shouldn't be offloaded as a project for the developer. Designer should specify things like focus order; 
-  Accessibility blue line (annotation kit)
-  Indeed has an accessibility annotation kit
-  Two main ways to bring in accessibility into your work as a developer
   -  Interact & engage with users who use assistive technology
   -  Automated tools, 
      -   Wave
      -   Ax 
      -   Pa11y
      -   Code linters
          -   Ax
          -   Eslint
          -   Axslint
-  Need a pipeline for complaints to reach product team
-  You can write an accessibility statement to encourage feedback about accessibility
-  Issue tracking - label accessibility-related items 
-  Accessibility bug-bashing days for fixing accessibility-related problems 
-  How do you prioritize? Where do you start? 
   -  Path of least resistance. Start with projects already started, already in progress. Begin tying in accessibility focus into those projects
   -  Gotta start somewhere, start where you know it'll be successful
   -  Value comes from telling people in the organization. Frame that first attempt as a pilot project and talk about it. How do you do this? Need metrics. What does success look like? Is there a baseline to measure against? 
-  Metrics
   -  Might use system usability scale (SUS)
   -  Accessible Usability Scale 
   -  Task Completion - ask someone to attempt a task and determine if they're able to do it. Include people with and without disabilities.
   -  Number of accessibility complaints & tickets; set goal for reducing by some percent each quarter
   -  Automated test coverage for accessibility
   -  What percentage of product has had user testing? 
-  Focus on things that are repeatable and improve reach / awareness. 
   -  Documentation
   -  Resource library
   -  Training, lunch & learns
   -  Accessibility guild
-  Need executive buy-in for scaling accessibility
   -  What works consistently? Video clip of person with disability trying to use product & struggling, a minute or two of this is effective. 
-  Rather than asking after the fact, *what's wrong?* reach out early and ask people with disabilities to contribute to creating an accessible product.
-  [PEAT](https://www.peatworks.org) - accessibility framework 
-  AA & AAA
   -  AA is a good standard to aim for; AAA implies greater customizations for specific groups of users with disabilities, and may make your product more accessible for that group at the expense of another group's experience
-  Accessibility improvements to your product affect not just users with disabilities but can improve the broader user experience; example: Netflix subtitles
## Conference Day 2
smashed.by/roll
