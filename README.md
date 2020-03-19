# SCSS Masterclass

(S)CSS Layout Masterclass: Flexbox & Grid

- CSS flex box appeared in context of solving manual positioning of boxes
- It's important to understand what problem that the technology has solved, instead of just learning stuff what other people think is valuable.

## Flexbox

- Only talk to the flexbox container outside, don't talk to the children. 
- Direct father controls the positioning of the children content
  ex) .wrapper is father of .box

### Flex-direction and axis

```css
.father {
	display:flex 
}
```

display flex sets default flex-direction as row

### **When flex-direction is row,**

![Basics1](https://mdn.mozillademos.org/files/15649/Basics1.png)

- Main axis is x-axis
  - justify-content move childrens on main axis
  - or, justify-content modify lines of main axis

![Basics3](https://mdn.mozillademos.org/files/15616/Basics3.png)

- Cross axis is y-axis
  - align-items move children on cross axis
  - or, align-items modify lines of cross axis

### **When flex-direction is column,**

![align10](https://mdn.mozillademos.org/files/15650/align10.png)

- Main axis is y-axis
  - justify-content move childrens on main axis
  - or, justify-content modify lines of main axis

![Basics4](https://mdn.mozillademos.org/files/15617/Basics4.png)

- Cross axis is x-axis
  - align-items move children on cross axis
  - or, align-items modify lines of cross axis

### When flex-direction is row-reverse ( or column reverse)

- Axis is the same, only the left-to-right sequential arraying is inversed as right-to-left.

### (Flexbox) order

- order is assigned according to main axis, sequentially
- default is 0

### flex-wrap

- wrap means to respect the size of the children, when window ran out of spaces
- nowrap means cram everyting in one father (line), even if sizes of children are shrunk

### flex-shrink

- enabled only when father doesn't respect the size of children

```css
.father {
	flex-wrap: unwrap;
}
```

- kicks in when window ran out of spaces
- default value is 1
- flex-shrink value 2 means it is 200% more likely to shrink than the other children

```css
.child{
  flex-shrink: 2;
}
```

### flex-grow

- enabled only when father doesn't respect the size of children

```css
.father {
	flex-wrap: unwrap;
}
```

- takes the space that is available to grow in the window
- default value is 0, which means that child will keep its size, doesn't take space that is available to grow
- flex-grow value 1 and 2 is proportional to each other: it grows twice more than the other children

```css
.child{
  flex-grow: 1;
}

.child:nth-child(2) {
  flex-grow: 2;
}

.child:nth-child(3) {
  flex-grow: 1;
}
```



## Concepts

- [x] flex-direction
- [x] order
- [x] justify-content
- [x] align-items
- [ ] align-self
- [x] flex-wrap
- [ ] align-content
- [ ] flex-grow
- [ ] flex-shrink
- [ ] flex-basis

## Grid:

- [ ] grid-template-columns
- [ ] grid-template-rows
- [ ] column-gap
- [ ] row-gap
- [ ] gap
- [ ] grid-template-areas
- [ ] grid-column-start
- [ ] grid-column-end
- [ ] grid-row-start
- [ ] grid-row-end
- [ ] grid-column
- [ ] grid-row
- [ ] grid-template
- [ ] justify-items
- [ ] align-items
- [ ] place-items
- [ ] justify-content
- [ ] align-content
- [ ] place-content
- [ ] justify-self
- [ ] align-self
- [ ] place-self
- [ ] grid-auto-rows
- [ ] grid-auto-flow
- [ ] grid-auto-columns

### Keywords & Functions:

- [ ] repeat
- [ ] fr
- [ ] minmax
- [ ] auto-fit
- [ ] auto-fill
- [ ] min-content
- [ ] max-content

## SCSS:

- [ ] Variables
- [ ] Nesting
- [ ] Mixins
- [ ] Extend
- [ ] Responsive Mixins

## To Clone:

- [ ] [https://besthorrorscenes.com/](https://besthorrorscenes.com/)
- [ ] [https://paint-box.com/](https://paint-box.com/)
- [ ] [http://10x19.co/](http://10x19.co/)
- [ ] [http://www.z-o-o.fr/](http://www.z-o-o.fr/) -> Referencing this website for FitCuration
- [ ] [https://schwartzmedia.com.au/](https://schwartzmedia.com.au/)
- [ ] [https://tolv.dk/](https://tolv.dk/)
- [ ] [https://rodicdavidson.co.uk/](https://rodicdavidson.co.uk/)
- [ ] [https://beige.de/](https://beige.de/)
- [ ] [http://donicaida.com/](http://donicaida.com/)
- [ ] [https://canalstreet.market/](https://canalstreet.market/)
- [ ] [https://wonhundred.com/](https://wonhundred.com/)

