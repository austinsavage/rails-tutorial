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

The same CSS can be expressed in SASS nested as:

```sass
.center {
  text-align: center;
  h1 {
    margin-bottom: 10px;
  }
}
```

However if you would like to use CSS selectors with attributes such as :hover, you can express that in SASS as:

CSS
```css
#logo {
  float: left;
  margin-right: 10px;
  font-size: 1.7em;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: -1px;
  padding-top: 9px;
  font-weight: bold;
}

#logo:hover {
  color: #fff;
  text-decoration: none;
}
```


SASS
```sass
#logo {
  float: left;
  margin-right: 10px;
  font-size: 1.7em;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: -1px;
  padding-top: 9px;
  font-weight: bold;
  &:hover {
    color: #fff;
    text-decoration: none;
  }
}
```