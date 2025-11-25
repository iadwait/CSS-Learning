# **✨ Flexbox Quick Reference**

### **Container (parent) properties**

| Property          | Short Meaning                    |
| ----------------- | -------------------------------- |
| `display: flex`   | Enable flexbox                   |
| `flex-direction`  | Row or column layout             |
| `justify-content` | Horizontal spacing (main axis)   |
| `align-items`     | Vertical alignment (cross axis)  |
| `flex-wrap`       | Allow items to wrap to next line |
| `gap`             | Space between items              |

---

### **Common `justify-content` values**

| Value           | Meaning                                        |
| --------------- | ---------------------------------------------- |
| `flex-start`    | Items left                                     |
| `center`        | Items centered horizontally                    |
| `flex-end`      | Items right                                    |
| `space-between` | First left, last right, even space between     |
| `space-around`  | Equal space around items (outer space smaller) |
| `space-evenly`  | Equal space everywhere (outer + inner)         |

---

### **Common `align-items` values**

| Value        | Meaning                      |
| ------------ | ---------------------------- |
| `flex-start` | Items at top                 |
| `center`     | Items vertically centered    |
| `flex-end`   | Items bottom aligned         |
| `stretch`    | Items stretch to full height |
| `baseline`   | Align by text baseline       |

---

### **Item (child) properties**

| Property      | Short Meaning                        |
| ------------- | ------------------------------------ |
| `flex-grow`   | How much item expands                |
| `flex-shrink` | How much item shrinks                |
| `flex-basis`  | Initial size of item                 |
| `flex: 1`     | Common shortcut for flexible item    |
| `align-self`  | Override vertical alignment per item |

---