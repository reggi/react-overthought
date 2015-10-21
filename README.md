# React Overthought

When I was learning React I came into it with a specific way of thinking. That I could encapsulate everything within the component, and make clean siloed components. This was very wrong, the result was this working example of a table with filtering and sorting. The thought problem with this way of thinking is that I wanted every component to behave like an actual native HTML element, and I wanted the DOM to save state. This is why when you sort or filter it uses the actual children nodes to do it, it doesn't pull the data and re-render from some external source. This was an interesting idea, but it fails when you want to actually make an app and bring in external data or connect mulitple components together.

I now embrace a more redux philosophy where there are super dumb components that expose their properties upward, where the root node delegates to the dumb components.

> Always a lesson, never a failure.

A Pen created at CodePen.io. You can find this one at http://codepen.io/reggi/pen/KdqdMW.
