📌 Behavior Explanation
1. .layout { display: flex }

Places sidebar + content side by side.

2. Sidebar has fixed width (250px)

It does not grow or shrink unless you set flex rules.

3. Main Content uses flex: 1

This means:

flex-grow: 1 → fill remaining space

flex-shrink: 1 → shrink when needed

flex-basis: 0 → start small then grow

So the main content automatically expands to take all extra space.