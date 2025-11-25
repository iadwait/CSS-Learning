flex-wrap
flex-grow
flex-shrink
flex-basis
Build a 3-card responsive layout
-------------------------------------------------

1️⃣ flex-wrap

Controls whether items stay on one line or wrap.

nowrap (default) → all items stay in one line

wrap → items move to next line when space is small

.container {
  display: flex;
  flex-wrap: wrap;
}

-------------------------------------------------

2️⃣ flex-grow

Controls how much a flex item can expand to fill extra space.

.card {
  flex-grow: 1; /* grows to fill space */
}
-------------------------------------------------
3️⃣ flex-shrink

Controls how much an item can shrink when space is low.

.card {
  flex-shrink: 1; /* default */
}
-------------------------------------------------
4️⃣ flex-basis

Sets the starting width of a flex item before growing/shrinking.

.card {
  flex-basis: 250px;
}
-------------------------------------------------
5️⃣ Common shortcut
.card {
  flex: 1 1 250px;
/* grow | shrink | basis */
}
-------------------------------------------------
