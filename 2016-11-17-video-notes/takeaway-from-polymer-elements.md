# Takeaways in Element Development

## Talk Information

Google IO 2016 - Google Chrome Developers  
[Youtube Link](https://www.youtube.com/watch?v=zfQoleQEa4w)  
Monica Dinculescu  
[@notwaldorf](https://twitter.com/notwaldorf)

### Description

Web components are the new shiny thing on the web, but what makes a good web component? 
How do you design a useful API that works for all of your users and all of their browsers? 
How do you make it render quickly and how do you teach people how to use it? 
After a year of working on the Polymer Elements, I've made sure to make all the possible mistakes 
so that you don't have to. This talk is about the things I've learned from that.

Watch more Chrome talks at I/O 2016 here: https://goo.gl/JoMLpB 
See all the talks from Google I/O 2016 here: https://goo.gl/olw6kV
Subscribe to the Chrome Developers channel at http://goo.gl/LLLNvf 

#io16 #GoogleIO #GoogleIO2016

## Main Points

1. API
1. Maintainability
1. Performance
1. Accessibility (a11y)

## API

Let's use the UNIX philosophy as an example of how to do good API design.
Let's use `<input>` as an example of bad API design.

#### It's ok to do **1 thing** and not do anything else

`grep` vs `input`

- grep does 1 thing
- input has 21+ types, doesn't do them all well

#### Composition: play nice with others

pipes vs nested HTML elements

- Pipes takes the output of one operation and passes it along to the next operation
- nested HTML doesn't always perform the way you expect.

```html
<select>
  <option>
    <span>option 1</span>
  </option>
  <option>
    <button>What?</button>
  </option>
  <option>
    <img src="lemon.png" />
  </option>
</select>
```

This will not render properly. The button and image will looked screwed up.
In the select, if you add an input, the browser will barf at you.

#### Extensibility: plan for the future

Elements nested in `<form>` vs. Polymer swipe element tries to swipe all things

Elements nested in `<form>` only allow certain tags to listen to change event.

#### Make no assumptions, have no regrets

- internal state changes. fire an event
- unix = process does a job and dies
- input, type="number" is a bad example because malformed values changes state
internally, and doesn't alert the user through an event.

#### Nobody actually likes surprises

You'll spend a long time debugging otherwise.

#### Polyfills

Don't jam a polyfill in an element. Let the developer decide that.  
But alert the developer they have to make that decision

TODO: Read the 17 principles in Unix Philosophy
-> it will help you write better APIs

## Maintenance

Maintenance earns trust

#### Semver

Semantic versioning builds trust.

-> 1.2.4

- "4" is a patch change. Accepting a patch change is a small fix that will not break your code
- "2" is a minor change. Adds things in API and generally should not break your code.
- "1" is a major change. Breaks existing code and developer must look at API changes.

#### Testing

Testing builds trust

- Test public API
- Private APIs should be denoted with "_", or "__" for private behavior
- Test accessibility - accessibility-dev-tools
- Test look and feel -> Loads of tools here
- Test element integration

Users need docs, so write the fucking manual

#### Performance

- Do one thing, do it fast
- focus on first paint

> Steve Orwell - on "First Paint"  
> Do less, be lazy

- *Do less*: Attach event listeners after paint
- *Be lazy*: Ripple all the components! (no, don't do that)

- Test your first paint performance
  - Two cheap methods
  1. `console.time` and `console.timeEnd`
  1. `performance.now`

#### Accessibility

> Accessibility is like a blueberry muffin  
> [@cordeliadillon](https://twitter.com/cordeliadillon)

--> It's hard to include accessibility because you have to do it E2E, from Start to Finish

Check out Rob Dodson's Talk @ Google IO 2016

- **Focus State**
  - keyboard only
  - tab index = 0
  - `document.activeElement`
- Use the platform! **aria** -> Speaks to us
