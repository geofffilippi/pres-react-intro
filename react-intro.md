## Geoff Filippi

### Senior Architect

---

# [DISH Network](www.dish.com)

---

# [Oildex](www.oildex.com)

A cloud service company for oil and gas

* 2 years

---

Formerly:

# [Time Warner Cable (Now Charter)](www.timewarnercable.com)

* 12 years

---

## Experience

## DISH Projects

* Microservices
  * Spring Boot
* Continuous Delivery
* Domain Driven Design
* React
 * Client-Side Components

---

## Experience

## Oildex Projects

* Rewrite 10+-year-old apps
* Angular 2
* Typescript
* Microservices
* NoSQL
  * Mongo

---

## Experience

<i class="fa fa-phone"></i>

* Worked on streaming media (Voice over IP), 6 years
* 5 million phone customers

---

## Experience

<i class="fa fa-video-camera"></i>

* Worked on video and streaming video, 4 years

---

## Projects

[twctv.com](twctv.com)

* Video streaming website
 * backbone.js
* Video streaming Set-Top Box (STB) web application

---

## Disclaimer

* Used AngularJS in production since 2015
* Used Angular in production since mid-2016
 * Angular 2
* Active member of the Denver Angular community
* A number of Angular talks and videos
 * TypeScript talks and video, etc.
* Currently work with teams that use Angular
* I know Angular better than I know React

---

## Disclaimer Disclaimer

* Currently work with teams that use React in production
 * Since Nov 2016
* Active member of the Denver React community
* Currently giving a React talk (video?)

---

## I'm Biased

### But maybe not that biased

* Co-orgainize HTML5 Denver
 * Big fan of the web
* Active member of the Denver JavaScript community 
* Changed front-end frameworks a few times

---

## Deciding between React and Angular

* Similar capabilities
* Try to learn both
* Development team should decide
* Angular makes more decisions for you
 * Decisions are hard
 * Allows you to override
* React requires your team to be better at making decisions
 * Follow the community

---

## Switching to React

> Applies to any switch

* Avoid switching existing projects
 * Both can be run together
* Switch on new project

---

## How to deal with churn

* Build smaller applications
* Everything does not have to be in one app
* Learn most popular frameworks and libraries
* Keep an eye on jobs/developer availability
 * Be willing to learn a new framework or train developers

---
---

# We will cover

* What is React?
* `create-react-app`
* Should I use React?

---
---

# [What is React?](https://facebook.github.io/react/tutorial/tutorial.html#what-is-react)

* JavaScript library for user interfaces
* Maintained by Facebook and Instagram
* Implements the View in Model-View-Controller (MVC)
* Can be used inside other frameworks
* Created by Jordan Walke a software engineer at Facebook
* Created in 2011
* Open-sourced in 2013

---

## Functional programming concepts used in React

* Declaritive
* Immutability
* Pure functions
* Higher-order functions
* Composition

---

## [Core React concepts](https://facebook.github.io/react/blog/2015/12/18/react-components-elements-and-instances.html)

* Components
* Elements
* Instances

---

## Some things to decide

* Router
 * `react-router`
* State management
 * `react`

---

## One-way data flow

> Properties flow down; actions flow up

---

## Document Object Model DOM

* Browser API
* Tree structure

---

## What does updating the DOM look like?

* CSS Recalculation
* Layout (reflow)
* Repaint
* Re-composting

---

## Virtual DOM

* In-memory cache of the DOM

> Only render sub components that actually change

---

## Why Virtual DOM?

* Assumes changing the DOM is slow
 * And will be slow for the forseeable future
* Assumes React can manage DOM changes better

---

## How can the Virtual DOM help?

Used properly:

* Allows developer to write app as if the entire view is rerendered on each change
* Detects what changed and what did not
 * Avoids unnecessary layout changes

---

## JSX

> JavaScript extension syntax

* Not HTML
* Superset of JavaScript
* Used to combine markup and application logic

---

## JSX Example

```
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}
```

---

## Components

* Create instances of elements
* `render()` returns a React element

---

## Component example usage

```
<ShoppingList name="Mark" />
```

---

## Elements

* Returned by component `render()`
* Describe component instances
 * Not actual instances
* Plain objects
* Can be nested

---

## Example Element

```
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
```

---

## Props

* Passed into Component
* Accessible in the `render()`

---

## Pure Functions

* `render()` does not mutate state
* output is only a function of input

---

## Instances

* References to the actual DOM
* React manages instances
* Created from elements

---

# [`create-react-app`](https://github.com/facebookincubator/create-react-app)

---

# Demo

---

## `create-react-app`

```
npm install -g create-react-app

create-react-app my-app
cd my-app/
npm start
```

---

## `creat-react-app` Tools

* Webpack
* Babel
* Autoprefixer
* ESLint
* Jest

---

* `npm start`
* `npm test`
* `npm run build`

---

## Other tools you will need

* `react-router`
 * Handle URLs
* `redux`
 * State management

---

## Code Walkthrough

---

## React Dev Tools

---
---

# Questions?

--

# Introduction to React

Slides from talk given on Mon 21st, 2017 at the HTML5 Denver Meetup Group.

>React is a popular JavaScript library from Facebook. React provides a view implementation for Web applications. 

>In this talk, Geoff Filippi (Senior Architect at DISH Network), will start by describing "What is React?". We will discuss how React uses components to build applications. Components can be implemented in JSX, an alternate version of JavaScript that allows mixing HTML-like markup and JavaScript. Input is passed into a component through props. Components return elements for display on the screen.

>We will have a look at `create-react-app`, a quick React application starter. `create-react-app` configures Babel to transpile JSX to JavaScript, and Webpack to build your application.


>Finally, Geoff will demonstrate how to create a simple React app.

[Markdown](react-intro.md)

This slideshow was written using [reveal.js](https://github.com/hakimel/reveal.js)

