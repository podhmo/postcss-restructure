# postcss-restructure

Don't use this.


memo:

```
/* style.css*/
/* @restructure(link) */

a {
  text-decoration: none;
}

/* @restructure(button) */
/* hmm */
.button {
  padding: 10px;
}

.pc .button.danger {
  background-color: red;
}
.pc .button.primary {
  background-color: blue;
}
```

to

```
/* tmp/common/link.css */
a {
  text-decoration: none;
}

/* tmp/common/button.css */
.button {
  padding: 10px;
}

/* tmp/pc/button.css */
.pc .button.danger {
  background-color: red;
}
.pc .button.primary {
  background-color: blue;
}
```
