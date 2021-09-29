# addIconOnLinkHover


```
<!-- HTML -->

<a href="https://www.google.com" target="_blank">Open link in a new tab</a>
```      

```
/* CSS  */

a[target="_blank"] {
    display: flex;
    gap: 0.05rem;
    opacity: 0.87;
}

a[target="_blank"]::after {
    content: url(assets/icons/newTabs.svg);
    opacity: 0.87;
}

@media screen and (min-width: 769px) {
    a[target="_blank"]:hover {
        opacity: 1;
        text-shadow: 0 0 2px rgba(153, 153, 153, 0.74);
    }
    a[target="_blank"]::after {
        opacity: 0;
    }
    a[target="_blank"]:hover::after {
        opacity: 0.87;
    }
}

```

## Résultat

