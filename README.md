# Midpoint Circle Algorithm

1. **Initialize the following variables:**
   - Center of the circle: \((cx, cy)\)
   - Radius: \(r\)
   - Starting point: \((x, y) = (0, r)\)
   - Decision parameter \(d = 1 - r\) (Initial decision value)

2. **Plot the initial points:**
   Plot the eight symmetrical points using the following coordinates:
   \[
   (cx + x, cy + y), (cx - x, cy + y), (cx + x, cy - y), (cx - x, cy - y)
   \]
   \[
   (cx + y, cy + x), (cx - y, cy + x), (cx + y, cy - x), (cx - y, cy - x)
   \]

3. **Loop until \(x < y\):**
   - Increase \(x\) by 1.
   - If \(d < 0\), update the decision parameter as:
     \[
     d = d + 2x + 1
     \]
     This means you move horizontally.
   - If \(d \geq 0\), update the decision parameter as:
     \[
     d = d + 2(x - y) + 1
     \]
     Then, decrease \(y\) by 1.

4. **Plot the new points** after each update using the symmetry.

5. **Repeat steps 3 and 4** until \(x\) is greater than or equal to \(y\).

6. **End the algorithm** once all points have been plotted.
