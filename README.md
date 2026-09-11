# WebGLLab3Part1

## Part 1
After replacing the lookAt() function with a translate() function, there was no change in the display. This is because in WebGL, setting the camera (eye) to be at positive 10 Z (moving it forward) and looking at 0 Z is the same as moving the objects in the scene to -10 Z (moving them backwards).

## Part 2
When both the lookAt() and translate() functions are removed, there is only black visible on the screen. This is because the camera and the lines are both at Z 0, so the camera doesn't see them. The camera needs to be moved away from the objects and be looking in the right direction for them to be drawn.

