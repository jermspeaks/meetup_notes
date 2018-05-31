# Resilient Web Design
## Chapter 2 Materials

### Notes

HTML is very liberal at throwing errors. If there's a tag it doesn't recognize, it will still display the content.

> This liberal attitude to errors allowed the vocabulary of HTML to grow over time from the original 21 elements to the 121 elements in HTML5. Whenever a new element is introduced to HTML, we know exactly how older browsers will treat it; they will ignore the tags and display the content.

> That’s a remarkably powerful feature. It allows browsers to implement new HTML features at different rates. We don’t have to wait for every browser to recognise a new element. Instead we can start using the new element at any time, secure in the knowledge than non‐supporting browsers won’t choke on it.

While some elments described the kind of content they contained, e.g. `<li>` `<p>`, other early elements risked making the markup language to showcase visual instruction, e.g. `<Big>` `<Small>` `<Font>`. These visual elements would easily swamp too many features.
> [Håkon Wium] Lie proposed a new format to describe the presentation of HTML documents: Cascading Style Sheets.

The proposal?

```css
selector {
    property: value;
}
```

CSS share's HTML's forgiving attitude to errors. It skips rules it does not understand.

Because of the nature of HTML and CSS, it's concept of compatibility is far reaching because developers can create new features even if other browsers do not support it yet.

---
Where you left off: https://resilientwebdesign.com/chapter2/#Killing%20it

### References

- [The Web is Ruined and I Ruined it]() by David Siegel
- [CSS Zen Garden]() by Dave Shea
