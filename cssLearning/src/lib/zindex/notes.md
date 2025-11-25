
# ⭐ Z-Index (Short Explanation)

**z-index controls which element appears on top when elements overlap.**

### ✅ When it works

`z-index` works **ONLY** when the element has a **non-static position**:

* `position: relative`
* `position: absolute`
* `position: fixed`
* `position: sticky`

These create a **stacking context**, allowing z-index to work.

### ❌ When it does NOT work

`z-index` does **NOT** work on:

* `position: static` (the default)

### ✔ Simple rule to remember

👉 **If you want an element on top, give it `position: relative` (or any non-static) + `z-index`.**

### ✔ Example

```css
.box {
  position: relative;
  z-index: 10;
}
```

### ✔ Overlap priority

Higher z-index → comes above
Lower z-index → goes below

---
