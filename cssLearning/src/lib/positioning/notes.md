POSITIONING
----------------------------------------------------------------------
SUMMARY
Static → Default position; elements flow from top to bottom in normal document order.

Relative → Shifts the element from its current position using top, bottom, left, or right. Other elements still treat it as if it’s in its original place.

Absolute → Element is removed from normal flow. Positioned relative to the nearest ancestor that has a non-static position; if none exists, it’s positioned relative to the <body>. Use top, bottom, left, right to place it.

Fixed → Element is removed from normal flow and positioned relative to the viewport (screen). It stays in the same place even when scrolling.

Sticky → Acts like normal/static/relative until the scroll reaches the threshold defined by top, left, etc. Then it “sticks” to that position inside its parent. Once the parent’s boundary ends, it stops being sticky.

----------------------------------------------------------------------

1. Static -> Default Position top to down placed
2. Relative -> You get access to top, bottom, left, right so you can position it as you want
3. Absolute -> 
🔹 How absolute positioning works
An element with position: absolute is removed from normal flow.
It is positioned relative to its nearest ancestor that has a position other than static.
🔹 Example
<div class="sibling1" style="position: relative;">I am relative</div>
<div class="sibling2" style="position: relative;">I am also relative</div>

<div class="absolute-child">I move to top of screen</div>

.absolute-child {
  position: absolute;
  top: 0;
}

✅ Result: .absolute-child ignores .sibling1 and .sibling2 because they are not ancestors.

🔹 Rule of thumb

Absolute elements are positioned relative to the nearest positioned ancestor in the DOM tree.
Siblings, previous elements, or later elements do not count.

----------------------------------------------------------------------
🔹 How static elements interact with other positions

Relative elements

Static elements see them in the normal flow at their original position, even if the relative element is visually moved with top/left.

Example: a relative element nudged down with top: 20px → static elements still behave as if it’s in the original spot.

Absolute elements

Absolute elements are removed from the flow.

Static elements ignore them completely — they don’t reserve space for them.

----------------------------------------------------------------------

4️⃣ fixed
What it is:

position: fixed removes the element from normal flow.

It is positioned relative to the viewport, not any parent.

It stays in place even when you scroll.
eg: - Naviagtion Bar we make it fixed

Example use case:
Toast notifications
Fixed navigation bars
Sticky buttons

----------------------------------------------------------------------

5️⃣ sticky
What it is:

position: sticky behaves like a normal static element initially — it stays in the flow and moves with the content.

When the element reaches the threshold you set (e.g., top: 0), it sticks in that position relative to its parent container.

Once the parent container ends, it unsticks and scrolls out of view.

eg - we want subheader to stick only till the content is there