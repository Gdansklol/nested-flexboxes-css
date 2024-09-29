# CSS - Nested flexboxes

exemple

```css
article {
  flex: 1 200px;
}

article:nth-of-type(3) {
  flex: 3 200px;
  display: flex;
  flex-flow: column;
}

article:nth-of-type(3) div:first-child {
  flex: 1 100px;
  display: flex;
  flex-flow: row wrap;
  align-items: center;
  justify-content: space-around;
}
```

1. flex-grow: 1: This means the flex item can grow to fill the available space in the flex container. If there's extra space, it will expand proportionally, depending on how many other items have a flex-grow value set.

2. flex-shrink: 1: This value indicates that the flex item can shrink if needed when the container is smaller than the total size of the items. If there isn’t enough space, it will shrink proportionally based on this value.

3. flex-basis: auto: This defines the initial size of the flex item. The auto value means the size of the item will be based on its content or width/height if specified, before applying the flex-grow or flex-shrink properties.

```css
.flex-container {
  display: flex;
}

.flex-item {
  flex: 1 1 auto;
}
```

-
