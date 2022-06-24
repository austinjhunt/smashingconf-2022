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
- If you are not using Figma for creating design systems, you should be. 
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
### Coffee Break 
[books](https://www.smashingmagazine.com/printed-books/)
[slack channel](https://smashed.by/slack)

### Robin Marx - Married to HTTP/3
@programmingart
- The long road to HTTP3
  - 2012 Google starts on QUIC
  - 2017 IETF adopts QUIC and HTTP-over-QUIC
  - 2018 Name "HTTP3" chosen
- What is HTTP/3?
- HTTP/3: 
  - head of line blocking removal
  - connection igration
  - better packet loss handling
  - tunable congestion control
  - better stream prioritization
  - built on UDP
- UDP does not require handshake
- QUIC integrates with TLS to allow both handshakes in one round trip 
- Zero RTT; do everything in first round trip 
- HTTP/3 fiddly
  - version negotiation
  - amplification prevention
  - large cert
  - retry
  - address validation failure
  - expired resumption ticket
  - non-idempotent request
- How to adapt your pages to H3?
  - very similar to H2, bit more relaxed
  - Fewer domains
    - consolidate on 1-3 connections in critical path
  - Less bundling
    - 10-40 files should be fine (inlining css still good tho)
  - Help browser
    - async/defer JS
    - preload/preconnect/priority hints/lazy loading
  - No server push 
  - **Easy way:**: use a CDN
    - Client & edge server connection uses H3, edge & origin still uses H2
    - Google CDN uses H3
    - Very easy to flip H3 switch
  - **Hard way**: doing H3 yourself

- The RSVP problem
  - If you send someone an invite to wedding, you want the guest to confirm so you can order food for them. 
  - H3 might
    - be blocked on network
    - not be enabled on server
  - browsers will only try H3 if supported
- Connecting to New domains (the alt-svc problem)
  - browser sends initial request over H1 or H2
  - server sends back alternative services header
  - browser stores alt-svc info in alt-svc cache
  - browser also tries H3 from now on, in parallel with H1 and 2 ("free" fallback)
- *Where did that present come from?* - identifying where the problems are
- Checking if HTTP 3 supported
  - httpcheck.net
  - docker image: ymuski/curl-http3
- Compare H2 to H3 performance
  - Google Lighthouse is excellent tool but not for network protocol testing
  - WebPageTest has built-in network throttling suite
    - Repeat View option: give alt-svc time to kick in
      - Both Chrome and Firefox switch to H3 *during* the first page load, not after
      - Both Chrome and Firefox still start with H2 in the repeat view
  - Chromium browser, customize command line options to force HTTP2 or HTTP3 and skip the alt svc flow, allows for apples to apples comparison
  - Low level data is available, just needs to be surfaced to higher level tools & views
  - Protocol performance is not low hanging fruit
    - Switching to H3 won't produce a drastic performance improvement for all users, will primarily improve performance for slowest 1-10% of your users
  - Time to first byte 
    - need to include DNS lookup times 
    - H2 used for very first page load, so very likely to incur a DNS lookup
    - H3 comes after, likely to have DNS data cached
    - Not a very fair comparison
    - Better: "Honest TTFB" excluding DNS request RTT 
- Summary
  - know what the feature does before using it
  - use a CDN
  - know the limitations of your tools; trust but verify 
  - hypothesize first, confirm with data
- eipiq21.github.com
- tech.loveholidays.com/making-loveholidays-18-faster-with-http3-1860879528a7
- Big reason to switch to new protocols is that they will evolve very quickly
  - Multipath
  - Web transport 

### Shubhie Panicker @shubie
#### Demystifying Leadership in the tech career journey 
- Tech Career Journey discussion
- Managing increasing scope & complexity of system(s) you are responsible for. 
- Complexity of a system defined by:
  - components of system
  - dependencies
  - needs of different stakeholders
  - failure modes of system and its integrations
- becoming senior
  - develop expertise in system
  - understanding dependent systems & vulnerabilities
  - manage needs of stakeholders
  - build solutions & robust integrations
- your work may be exemplary but if it's narrowly scoped you may not be considered for leadership 
- complexity beyond senior **increases dramatically**
  - complexity of system components
  - complexity of dependencies
  - needs of different stakeholders
  - learning to work with people becomes very helpful at this stage
- **Systems thinking**: a way of exploring and developing effective action by looking at connected wholes rather than separate parts
  - Step back and consider whole system and interactions between parts
  - Reflect, get additional perspectives
  - Identify behavior changes to try; might be a new process for the team(s), will take time to determine if it works well
- Managing systems of increasing complexity summary
  - Not-yet senior
    - component that is part of larger system
    - provide technical solution to given problem defined for you
  - senior
  - beyond-senior
    - systems-thinking. significantly more complex, responsible for components and their connectedness. 
- Discomfort fuels growth
- Who are you trusted by?
  - Follow leaders wisely.
  - Do they believe in me?
  - Can they support my growth?
  - Do I believe in them?
  - Aree they growing in scope or influence? 
- Function areas & Skills
  - Tech
    - core technical skills; e.g. engineering, UX, etc.
  - Project management
    - steer execution, coordinate teams, manage timelines and budgets
  - Product management
    - define product with market understanding, shape strategy
  - People management
    - manage technical people, promote productivity, grow careers
- Rare to find a team / organization that is equally strong in all functional areas
- Where are your interests/skills as they relate to those 4 areas?
- Grit: The Power of Passion and Perseverance (Book by Angela Duckworth)
- 2 challenges to resilience. Resilience is ultimately what keeps you in the game & dealing with burnout, and **staying in the game is critical to your tech journey. **
  - fear
  - fatigue. need to recharge!
- Writing down your goals helps you to build resilience. 
- Don't get too comfortable. Your goals & your scope of work should be stretching you. Discomfort fuels growth. 
- Be honest with yourself. Where am I with these things and where do I want to go? 
- Should managers in the tech arena have deep technical skills?
  - Need to be able to intelligently speak to the tech. But more important to have tech leads that you trust with whom you can hash out technical issues even if you don't have the deep technical skills. 
- How long does it usually take to become proficient/feel comfortable in a new role?
  - You should always be a little uncomfortable. 90 days to 6 months to start feeling confident. 
- Can you grow in your career/climb the tech ladder without having to manage people?
  - Certain companies actually require you to manage people as you get promoted. 
- How quickly do you think it's okay to expect a promotion in tech? 1.5 years-2.5 years is common at Google if you're not a senior yet. Once you're a senior, 2.5-3.5 years generally to get promoted at Google.


### Miriam Suzanne: [Codepen](https://codepen.io/miriamsuzanne) - OddBird - @terriblemia
#### Styling the Intrinsic Web
Member of CSS working group, W3C 
- CSS exists for two primary reasons
  - CSS describes reusable objects
  - CSS describes responsive styles
- On every HTMl element, every CSS property must have exactly one value
- Web for all. Web on everything. - web mission statement
- Everyone has input. User agents, devices, authors.
- There are too many variables to consider when designing for the web. The point of CSS is to make it so you don't have to worry about all of them. 
- Our job when writing CSS is to define a few constraints and let the language figure out the rest because it's smarter than us. 
- Cascade filters out. Inheritance fills in. 
- Cascade Origins
  - user agent (browser)
  - user (preferences)
  - author (site)
- If conflicts arise the user should have the last word
- !important is a balance of power between origins ; it's there to protect styles from someone coming along later and taking away something that's important. Not there for us to override stuff 
- Selectors
  - \* (universal)
  - type
  - .class & \[attr]
  - \#IDs
##### Cascade Layers
- give you control over your part of the cascade
- creating layers of specificity; you can do this with the @layer rule
- can create as many layers as you want & put styles in each one 
- layers take precedence over specificity
- can establish layer order up front to establish precedence;
  - @layer generic, elements, objects, components, overrides;
- unlayered styles have the highest priority by default
- long term we're moving toward putting every style in a layer because it's clearer
  - you can nest layers
    - can use dot notation to access nested layers
  - layers override, importance protects
  - Example 
    - @layer base, theme, state;
    - want state styles to override theme styles; want theme styles to override base styles
##### Scoped Styles
- different from shadow-dom encapsulation
  - shadow-dom encapsulation is more of a hard boundary, nothing can get through
- scoped styles is more of a soft boundary; global styles can still come through/be inherited
- @scope
##### Container Queries
- problem: layout loops because of normal flow
  - content sizes parent and parent sizes content
- 2020 proposals:
  - david baron: @container
- components need to lay out the children & not be laid out by their children
- can't ignore the content entirely though
- we need inline size containment
- dino's paradox; in order to get somewhere, you have to go halfway then halfway then halfway then halfway, but in that case you wont ever get there
- container-type: inline-size;
- contain: inline-size
- can nest containers as much as you want;
- Finding Containers
  - match every element and find nearest ancestor that has the right container type 
  - Later this year and into next year all major browsers will support container queries
  - Container query units
    - cqw | cqh | cqi |cqb | cqmin | cqmax
  - @container style(--colors: invert) {...} 
  - @container state(is-stuck) {...} 

### Elliot Jay Stocks @elliotjaystocks
#### Typography for the People 
- Magazines
- [8 Faces](https://8faces.com)
  - 8 issues; interview 8 designers, ask for 8 favorite typefaces
- [Lagom](https://readlagom.com); 10 issues; lifestyle magazine
- [King Sejong, Korea](https://en.wikipedia.org/wiki/Sejong_the_Great)
- Invented writing system (hangle writing system for Korean language); shapes & letter forms give hints about how to pronounce words
- [Sexy Web Design](https://elliotjaystocks.com/blog/sexy-web-design)
- Did redesign for smashing website
- [Insites: The Book](https://www.goodreads.com/book/show/16031919-insites)
- ClearSans
- [Maido](https://medium.com/@elliotjaystocks/behind-the-scenes-of-maidos-rebranding-7359bec4c763)
- [Google Fonts Knowledge](https://fonts.google.com/knowledge)
- [Components.ui](https://componentsui.com)
We often judge success based on impression-based metrics, but we should be focused on expression-based metrics. What do people actually care about?

### Cassie Evans
#### Animating the Impossible
- Magic card trick introduction
- Animating some really tricky UI stuff involving responsive layouts
- [GreenSock](https://greensock.com/)
- [codepen.io/cassie-codes](https://codepen.io/cassie-codes)
- [gsap](https://greensock.com/gsap/)
- the world that HTML elements live in is infinite and unknowable; the world of SVGs is predictable
- UI animation can be integral to understanding an interface for people
- vision
  - rods in peripheral vision, more sensitive to movement, "hey! over here"
  - cones in central vision
  - more neurons analyze stuff in the central vision rather than peripheral vision
  - we see a lot less than we think -> inattentional blindness. magicians take advantage of this
  - change blindness -> failure to notice an obvious change; UCI study re: spotting the difference
  - refreshing the page means users have to reorient themselves; better to have smooth page transitions without interrupting the interface
- after all your styles and JS is loaded, browser goes through 3 steps
  - layout -> paint -> composite
  - this is very fast/efficient, but if you animate elements of layout or paint steps (e.g. left, right, width, background color), not as efficient/fast
- you need to make it appear to user that element has not moved even if you've moved element to entirely new place and put it back again with FLIP. Avoid layout reflows.
- On parent: FLIP
  - First
  - Last
  - Invert 
  - Play
- On children: FLOP
  - First 
  - last 
  - offset 
  - parent
- in Layout stage
  - first el.getBoundingClientRect()
  - then move element to new position
  - then calculate how far element has moved
- before Paint step, move element where it needs to be 
- use motion to signal change
- SVGs are a great way to get started with animation


## Conference Day 2
[smashed.by/roll](https://smashed.by/roll)
### Mystery Speaker: Addy Osmani @addyosmani
#### Life Lessons & Introspection
* First do it, then do it right, then do it better. Don't get lost in perfectionism. Ship when it's good enough. 
* Time is your greatest asset. Use it wisely. Technical mastery implies a high ratio of value shipped to hours worked. Work on the right things. 
* Understand what gives you energy & what takes it away. It

##### Nostalgia
##### Introspection
- 5-prompt framework for introspection
  - What do I want?
  - What am I avoiding?
  - What am I grateful for? 
  - What am I afraid of? 
  - What are my strengths/faults?

### Harry Roberts @csswizardry
#### Get Your Head Straight
- cardiocentric theory
- key concepts
  - HTML parsed line by line
  - the `<head>` is the biggest single render-blociking part of your page
- [csswz.it/gyhs-baseline](https://csswz.it/gyhs-baseline)
- don't be big-headed; if it doesn't need to be in the head, remove it. has a major performance ipmact 
- self-host whatever you can; [csswz.it/self-host](https://csswz.it/self-host)
- pro tip for self-employed devs: never tell clients what you did, but the outcome of what you did 
- Move CSP data
- Metadata about the page goest first
  - tell the browser how to deal with the page, e.g. viewport
- Put your synchronous JS before CSS 
  - CSS blocks execution of subsequent JS
- avoid @import in CSS files, bad for performance; removing it allows for more complete parallelization
- SEO and Social Goes last. It's asynchronous so really it doesn't matter where it goes. If Google Bot can't find your meta tags, it can't find your body either. 
- A New Order: [csswz.it/gyhs-fixed](https://csswz.it/gyhs-fixed)
- [csswizardry.com/ct](https://csswizardry.com/ct) - tool for assessing head tags
- [csswz.it/smashingdevtools](https://csswz.it/smashingdevtools)
- [harry.is/for-hire](https://harry.is/for-hire)
- favor HTML whenever you can rather than depending on JS to populate the DOM


### Vitaly Friedman
#### Designing for Complex UIs
- working in complex environments may involve dealing with visualizing tons of data in different ways
  - filtering, view changes, different perspectives
  - ability to create understanding out of data is something that we are often missing
- Some digital products are inherently complex bec of deeply intricate environemnts in which they operate. They are designed for expert users operating in a knowledge domain. 
- Complex interfaces are composed of a core set of reusable components, e.g. multi-level navs, cards, dashboards charts, timelines, data views, maps, auth, privacy, etc.
- Design KPIs; rare?
  - With DKPIs, the design is always driven by constraints and user-centric goals. The outcome is evidence-based design. Without subjective or random decisions. 
- How to test?
  - Task instructions. Give people tasks to execute within your design. Goal is to get 80-90% success for all of the tasks. 40-50 people. 
- To get to high success rates, as we iterate, test exactly the same 15 top task instructions with eact same segments of audience over time at least every 4-6 months. 
##### Navigation
- dealing with copmlex menus
  - mega-sites usually extremely large, many levels deep, made of many micro-websites, etc. mega menus are disgusting. 
  - Hover tunnels. 
- Amazon triangle path.
- Avoid hover menus! Better to have click menus. Works as expected on mobile as well. 
- Sideways breadcrumbs. Often problematic & implemented incorrectly. 

Filters.  Dell's filters are rough. Drive users through options in predictable way, don't show all options at once. Decouple the results from the filters. Don't slow down your users when they don't want to be slowed down. 

Carousels. How do we make them better? 
Make sure you have a bright, clear mapping between the indicator and what is supposed to happen. Like, don't show a slider bar if you have to swipe across the screen to trigger something. 

Infinite Scroll. Lots of issues, no sense of current state. Maybe use a "continue here later" button, that links to the section of the infinite scroll. 

[Smart Interface Design Patterns](https://smart-interface-design-patterns.com/)

### Sophie Tahran @stahran
#### Designing with Words
- UX writing lead; Conde Nast
- New Yorker, invision, lyft
- taqueria cancun - SF food recommendation
- What UX writing is
  - content design
  - practice of designing useful content that guides users through digital experiences
  - product design through a written rather than visual lens
  - work primarily in figma
  - product design, figma, designs
  - repetition is good; in UX writing, a different word signifies a different action
  - never sacrifice clarity for sake of concision
- Why it matters
  - we're moving into a world where every piece of content needs to be created strategically
  - leads to 
    - better products
    - better UX
    - better brands (build trust, loyalty, credibility)
- Creating your process
  - generative research
  - support tickets
  - competitors
  - Reference other people's language to guide your own language
- Applying best practices
  - use & ! ; - sparingly 
  - avoid arbitrary capitalization

### Dan Rubin
#### We Don't Talk Anymore
##### Teamwork
We're still debating whether designers should learn to code. 

"Our modern family gathering, silent around the fire, each individual with his head buried in his favorite magazine." Journal of Education

Our tendency toward isolation is a pattern, not new. 
We're really good with building walls.

We long for human connection yet close ourselves off from direct interaction. 

Brene Brown, The power of vulnerability: "Connection is why we're here."
Why do we separate & define ourselves & others?

Roles help us create a mental model of the world. We start defining our differences early.

The language of separation is embedded in our world. E.g. male & female idea embedded everywhere, people, plugs. Schools separate us by age, subject, etc.
We define behavior as "child-like"/"grown-up".

Defining roles allows us to assign responsibility.

Roles important for teamwork. Yet we tend to allow roles to separate us rather than pull us together.

Montessori encourages collaborative play across age groups.
##### Think small(er).
Small startups tend to behave this way.

Smaller teams tend to come with more active involvement by the members. Less focus on isolation & separated roles. More focus on common goal.

As teams grow, segmentation becomes more common, communication becomes more difficult, relationships change. 

GoreTex example. - when a department grew over 150 or so people ([the dunbar number](https://en.wikipedia.org/wiki/Dunbar%27s_number)), department got divided. Problems with communication & relationships resolved by creating smaller groups. Dunbar number not absolute, but helps us to think smaller.  

[Big Spaceship Agency in Brooklyn, NY.](https://www.bigspaceship.com/). Big Spaceship Manual: *"Try not to over-formalize communication. There's no need to send an email to the person sitting one desk (or Slack message) away."*

Often the systems / processes we implement to scale up end up getting in the way of productivity and human-ness. E.g. using email for documented communication at the expense of quick in-person communication. 

Consider how your approach to defining roles might be affecting your team's ability to achieve their goals.

Inherent value studies: focusing on features of a product when you're working on improving for a future version; focuses on things that are working well that you want to protect. This same thing should be applied to scaling up team sizes. What's working well with the small team? Protect that. 

How do you reorganize communication to avoid flooded chatty channels particularly in a remote work environment?
  - Comes down to setting boundaries. 


### Jhey Tompkins - DevRel Engineer @ Google
#### Take your skills to the moon with creative coding
This was primarily a demo of many codepen projects. 