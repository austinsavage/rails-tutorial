# Chapter 5: Filling in the Layout

## SASS

### Nesting
```css
.center {
  text-align: center;
}

.center h1 {
  margin-bottom: 10px;
}
```

The same CSS can be expressed in sass nested as:

```sass
.center {
  text-align: center;
  h1 {
    margin-bottom: 10px;
  }
}
```