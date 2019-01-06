# Sprite Test

A test to benchmark sprite rendering performance on various platforms.

This application simply renders a moving background with a variable number of animated sprites on top. A counter displays the current number of sprites being rendered. The counter increases until the framerate falls below 60 frames per second, then decreases until the ideal framerate is restored. Each time the counter changes direction, the counter speed decreases. Eventually, the counter stops changing, providing an estimate of the maximum number of animated sprites that can be rendered atop a moving background.
