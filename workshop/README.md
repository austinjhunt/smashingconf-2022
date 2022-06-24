# Smashing Conference 2022 
## Brad Frost - Workshop - 6/23/2022 - @brad_frost
### Creating & Maintaining Successful Design Systems
[https://atomicdesign.bradfrost.com](https://atomicdesign.bradfrost.com)
[patternlab](https://patternlab.io)
[styleguides.io](https://styleguides.io)
[style guide guide](https://bradfrost.github.io/style-guide-guide)
- clients
    - united
    - pfizer
    - ppg
    - petsmart
    - comcast
    - conde nast
    - cosmopolitan of LV
    - athenahealth
    - nasdaq

- key notes
  - use [storybook](https://storybook.js.org/)!
  - need front end devs, not just full stack 

- todo:
  - sell 
  - kickoff
  - plan
  - design/build
  - launch
  - maintain (hardest part)

- members of workshop
  - louisiana state gov't ux & ui lead


#### MORE
We're aiming for more customers, more languages, more content, more devices, more modalities,

#### What is a design system?
A design system is the story of how your oganization designs and builds digital interfaces. 
[Blog Post](https://bradfrost.com/blog/post/design-systems-are-for-user-interfaces)

We need a clear boundary between what's in the design system and what is not. 

Design system cares about content, brand, accessibility , personas , product needs, internationalization, personalization, performance, analytics, testing, voice & tone, copywriting, but it is not a catch-all for all of those things.

What is a design system consist of from an asset standpoint? 3 legged stool:
- Design libraries
- Code UI component libraries
- Reference website

[Medium Article on design systems](https://medium.com/design-systems/)

It's assets, people, processes centered around owning, governing, and managing user interfaces. 

#### Sell

##### Benefits of Design Systems
- promote UI consistency & cohesion
  - Jakob Nielson: *consistency is one of the most powerful usability principles: when things always behave the same, users dont have to worry about what will happen. instead, they know what will happen based on earlier experience.*
- faster production! one of the most measurable benefits
- make dark corners not so dark anymore! Federico Holgado - mailchimp status page improvement. 
- Design system carries the burden of the boring. 
  - Don't build same thing over and over. Focus on more worthwhile tasks like accessibility, performance, & iteration. Enables you to respect people's time & energy. 
- higher-quality production = teams can focus on higher-level tasks
- easier to test = more repsonsive, performant, accessible experiences
- shared vocabulary = more time collaborating & less time in meetings
- useful reference = essential resource & hub for best practices
- future-friendly foundation - modify & extend over time


[css stats](https://cssstats.com) - spits back all of your CSS

What can you weed out?
- 50 shades of grey
- close-but-no-cigar color matches
- font sizes
- font families

Interface Inventory Group Activity
1. Round up the troops
2. Prepare to screenshot
   1. bit.ly/interfaceinventory
3. Do the inventory, assign categories to teams, e.g. global, image types, icons, navigation, forms, buttons, interactive components, etc
4. Discuss findings, enables you to start articulating what is being used, why it's being used, and why certain things don't make sense. 
5. Present finidngs to execs, move fast & broad, 30 minutes max. Let decision makers know that things are disorganized and a design system can provide value. 
6. Regroup & next steps.

Functions of interface inventory:
 - documentation of design patterns
 - point out inconsistencies
 - helps buy-in from organization
 - establishes scope of work
 - informs pilot project selection
 - is the genesis of shared vocab
 - lays groundwork for future pattern library 


Note: include 3rd party sites that are branded like your organization. That counts as inventory. 

##### Performance Check
WebPageTest - allows you to show how your website's performance compares to competitors
WPO stats
axe DevTools - Web Accessibility Testing 
Accessibility-related legal liability can be a good tool to leverage when trying to sell a design system. 


#### Kick Off
What happens if you **sell** successfully? Kicking off the design system.
##### Research & Interviews. 
Some questions: 
- what are you workingon now?
- what are your priorities?
- what's a day in the lfie look like?
- can you describe your current workflow? what works well? what does not?
- what aspects of the workflow could be improved?
- if you could change one thing what would it be?
- what are the relationships like within your team?

###### Stakeholder & user interviews
- round up diverse group of stakeholders, colleagues, users, who would be impacted by design system
- ask questions about their experiences (good & bad) using the web site
- synthesize themes in prep for kickoff
**Priorities Workshop**
dotdash - formerly about.com
whiteboarding / sticky note sessions - what parts of the design system are most important? examples:
  - raise/maintain ad revenue
  - build lasting design foundation
  - delight readers
  - impress market and industry
  - create memorable and differentiated brand
  - increase ad flexibility
  - craft an effortless reading experience

Helps to create a broad consensus about what design system needs to do. 

#### Plan
What are we making? Who's going to do it? How? 
- Important Split
  - Design system makers
  - Design system users

When you're getting something off the ground, a small team is what you want. 5ish people or less. Want small group of smart, autonomous people who move quickly. 

Out of all the products/sites you have, look at each of them and identify the best candidate for starting your design system. What's the best lens? Chat? Academic program pages? Catalog?


Once you identify the product/site for your design system pilot project, you can build it out and validate it (i.e. these components can at least build this one product/site), and then you can use that pilot project to communicate the value of the system. 

If the design/build phase has already started the ship has sailed. Nearly impossible to implement a DS after that process is in motion.


Criteria for choosing pilot projects
- potential for common components & patterns; does the pilot have many components/patterns that can be reused elesewhere?
- Scope - is this work accomplishable in our pilot timeframe of \[3-X] weeks?
- Technical feasibility & independence - how simple is the technical implementation? is a large refactor or migration required?
- Available champion - will someone working on this product be a good guinea pig, see it through and then celebrate/evangelize the DS? 
- Marketing potential - will this work excite others to use the design system?

This pilot project will produce a design system package which you can incrementally feed through other products/sites. 

- Design Brief
  - define goals, principles, scopes
  - goals: spell out business and user needs
  - definition: what needs to be included in DS?
  - principles: what are guiding principles?
  - plan of attack: timeline & scope
  - circulate with team, interviewees, other stakeholders; keep door open for conversation & prevent / avoid swoop and poop

- Design Principles
  - Split:
    - Process principles
      - make the best thing the easiest thing
      - design for grab it quick efficiency
      - design for contribution and community
      - crowd-proof markup 
      - fit the workflow
      - just enough docs
      - tech agnostic
      - embed brand in code
      - conssitent, not homogenous
      - opinionated defaults
      - make people smarter just by using it (elevate design best practices)
    - Product Principles
      - just enough interface
      - strong/direct
      - speed is a feature
      - adaptable desnity
      - safety always
      - no tricks or stunts
      - recycle, reduce, reuse

Creating design principles: [articles.uie.com/creating-design-principles](https://articles.uie.com/creating-design-principles)
  
##### Consider your approach
Be deliberate, organized, intentional with DS. Intentionality & organization allows for the velocity of creation. Atomic design is good but if no one knows where the components are then you're still moving slow. 

**Atomic Design Layers: From Abstract to Concrete**
1. Atoms: input fields, buttons, labels
2. Molecules: labeled input field with submit button
3. Organisms: header organism containing labeled input field with submit button for search
4. Templates: multiple organisms; content scaffolding / layout
5. Pages: built with templates, putting real content within it ; this is what you share when you finish the pilot project; this is where you can validate & test different use cases

[Frank Chimero: The Shape of Design](https://shapeofdesignbook.com) - switch between abstract & concrete/details to see how small changes impact larger system continuously, like a painter

*Atomic design is a helpful mental model, not rigid dogma.*

Third-party design systems
- pros
- provided libs for design & dev
- quickly get up and running
- CONS
  - lookalike issues
  - limited customizability
  - limited by library's roadmap and conventions
  - library likely does not provide every UI solution
  - vendor lock-in
  - can create rifts between design and dev. devs will pick libraries as a dev expediency without telling designers. 
  - DESIGN TEAM SHOULD BE AWARE OF DESIGN CHOICES MADE BY DEVELOPERS.

When it's okay to use third party design system, e.g. material ui
- quick prototype / trial needed
- limited/no resources
- limited brand/design needs
- don't need to support multiple technologies/products


When to plan, build and launch custom design system
- creating system to serve as org standard
- planning on maintaining digitial products in long term
- have resources (either now or in the future)
- want to achieve specific brand and design goals and results
- need to suppport multiple products and/or technologies
- want flexibility to extend and customize to meet organization's needs

[Frontend guidelines questionairre](https://github.com/bradfrost/frontend-guidelines-questionnaire)
[CSS Guidelines](https://cssguidelin.es/)
[BEM-style CSS syntax](https://css-tricks.com/bem-101/)

[Plop](https://plobjs.com) - allows you to enforce consistency across your components

#### Design & Build 
- Minimum viable artifacts
  - often don't even need to be artifacts. could be a conversation. "here's a description of what i want: xyz"
- Element collages - exploring the brand direction - [example](https://dribbble.com/tags/element_collage)
- Collaboration & communication > deliverables

Design Subsystems
- **Design tokens**; once these are in place, they're very stable. Refer to conference talk notes for more info on design tokens.
  - theme-[token category]-\[background/content/border]-\[token subcategory/type]-\[optional-state]
    - Example: theme-coolred-background-primary-hover

[https://designsystem.quickbooks.com/foundations/color-palette](https://designsystem.quickbooks.com/foundations/color-palette)

Difference between dark mode and inverted; "knockout" property on component to render an inverted style for accessibility purposes. E.g. your text may generally be black but if it doesn't show up well enough on a dark background component, knockout property inverts dark text to light text on dark background


[Gridless Design](https://gridless.design)
[8 Point Grid System](https://medium.com/swlh/the-comprehensive-8pt-grid-guide-aa16ff402179)
[Project Healthy Minds Netlify Storybook](https://phm.netlify.app/?path=/story/atoms--design-tokens)

- [Snowflakes, recipes, design system components](https://bradfrost.com/blog/post/design-system-components-recipes-and-snowflakes/)
  - Recipes are product specific configuration/combination of design system components to serve a specific purpose, not part of the design system itself because it doesn't need to be widely used 

API Design
- use `variant` consistently across your component library to indicate stylistic differences for functionally consistet components
  - e.g. `variant="primary", variant="secondary", variant="link"` etc
- use `size` property consistently
- why?
  - more efficient dev & design
  - shared vocabulary
  - future changes are easier
#### Launch
Spectrum of integration
least integrated => static => frontend reference code => consumable components (used via import) => most integrated
`npm publish` -> publishes design system package in dist/* 
- allows you to manage design system as a separate product, which it is
- [nathan curtis](https://medium.com/@nathanacurtis), good resource

##### Documenting design systems
- reference website 
  - separate from dev documentation and designer documentation
  - should be a public website
    - product owners, copyrighters, QA engineers, developers should all use this 
  - [zero height](https://zeroheight.com) - design system content management system that does all of this documentation for you 
      - Increase adoption of your design system
      - can embed storybook inside it 
      - code source of truth stays the code source of truth
      - design source of truth stays design source of truth
      - they both get funneled into zero height
    - [primer.ppg.com](https://primer.ppg.com)
  - good place to link out to reasoning/data behind the design system, e.g. why was a component designed this way?
  - Contributing guidelines are important
    - where to go for help, how to contribute, here's how it works, links to other things
  - [styleguides.io/podcast/nathan-curtis](https://styleguides.io/podcast/nathan-curtis)
  - [styleguides.io/podcast/jina-bolton](https://styleguides.io/podcast/jina-bolton)
  - Having a public-facing design system can really help with **recruitment**
  - [lightning design system](https://lightningdesignsystem.com) - Salesforce's design system pulled in new recruits to their team
  - 

#### Maintain
- not good: design & development -> product -> style guide
- when we develop websites, documentation tends to be an afterthought after the website itself
- very common for product to reach a point where it no longer reflects the documenation 
- how do we create successful design systems that will stand test of time?
  - put the design system **in the path** of success. if it hangs out on the side, it's gone. it needs to contribute to the design & development. 
- good: design & dev -> design system -> product & style guide

Design System Makers
- have a birds-eye perspective of entire ecosystem
- the ones responsbile for maintaining the design system
- approve changes
- work with users and business to make sure it's addressing the product needs
- need to establish a pattern-driven, cross-disciplinary workflow. THESE ARE THE PEOPLE THAT NEED TO WORK THIS WAY. THEY ARE PROVIDING COMPONENTS & KITS THAT OTHER TEAMS ARE CONSUMING. 

Design System Users' perspectives need to also be present in the creation of the DS
- provide on the ground perspective focused on specific applications
- may also be makers, separate development teams, junior-level devs, partner agencies, external dev shops, third-parties 
- should coordinate with makers to make sure system is addressing their needs
- may be widely distributed and process may be extremely waterfall


Design System Team Makeup
- product owner, needs to be really good with people
- product manager, especially for responding to people's feedback about the launched system
- design lead, high level, type system/color system, sort of senior level; someone who is owning the design architecture
- production designers, doing actual work in figma library, more head down involvement taking direction from design lead
- tech lead, leading development, CSS, component architecture
- front-of-the-front-end developer(s);  good to have at least 2 developers for decent velocity

[Design System Team Models](https://medium.com/eightshapes-llc/team-models-for-scaling-a-design-system-2cf9d03be6a0)
- Centralized ; this model helps to capture the birds-eye perspective, but it has risk of losing the on-ground/in-the-weeds perspective. Team may end up working from an "ivory tower", not solving actual problems, silo.
- Federated; *"We need our best designers on our most important products to work out what the system is and spread it out to everyone else. Without quitting their day jobs on product teams.... Such a committee federates a system’s design direction to a representative, empowered subset of designers and leaders designated to collaborate on the system for a period of time."* - Nathan Curtis
- Cyclical; *The Design System informs our Product Design. Our Product Design informs the Design System.* - Jina Bolton

[Design System Council](https://medium.com/related-works-inc/the-people-part-of-design-systems-a5b54eea24f4) - Magera Moon

Design system cares about the user research insofar that it affects the user interface, don't need an owner of user research on the design system team; design system team consumes the output of that research from another team. 


##### Governance
*Set it and forget it.*
People often think things are set in stone once design system is launched, but it's not. Change is the only constant in life. 

[Vanilla Pattern](https://coggle.it/diagram/V0hkiP976OIbGpy8/t/vanilla-pattern)


