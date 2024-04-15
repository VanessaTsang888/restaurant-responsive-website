# 117. Building the Meals Section - P3

The Learn More btn on the header:

Transition all properties not just the bg colour so it looks btn more fluid on hover.

```css
.btn:link,
.btn:visited {
  transition: all 0.3s;
}
```

## Short keys

select the element, then hold-down the alt key and use the arrows keys to select the other lines of code you need. Then we can write in multiple places.

## Check mark icon

1. search and choose the check icon: www.ionic.io/ionicons
2. Past the code within all the list items.

### Styling icons

To remove the default bullets as we want to use the check icon instead:

```css
.list {
  list-style: none;
}
```

```css
.list-icon {
  width: 3rem;
  height: 3rem;
  color: #e67e22;
}
```

To make the list items vertically align we use css flex-box.

```css
.list-item {
  font-size: 1.8rem;
  display: flex;
  align-items: center;
  gap: 1.6rem;
}
```

To apply equal spaces between each list we use: `flex-direction: column`

```css
.list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 1.6rem;
}
```
