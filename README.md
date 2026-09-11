# WebGLLab3Part1
Morgan Lincicum
09/11/26

## Step 1
After replacing the lookAt() function with a translate() function, there was no change in the display. This is because in WebGL, setting the camera (eye) to be at positive 10 Z (moving it forward) and looking at 0 Z is the same as moving the objects in the scene to -10 Z (moving them backwards).

## Step 2
When both the lookAt() and translate() functions are removed, there is only black visible on the screen. This is because the camera and the lines are both at Z 0, so the camera doesn't see them. The camera needs to be moved away from the objects and be looking in the right direction for them to be drawn.

## Step 4
When the canvas dimensions are changed to width="512" height="256", the display becomes shorter and the green line becomes longer than the red line (when before they were equal length). When the canvas dimensions are changed to width="256" height="512", the display becomes narrower and the red line becomes longer than the green line. However, when the perspective() call is changed so that the aspect ratio is canvas width / canvas height rather than just 1.0, at both sizes the lines appear as the same length (correct).

## Step 10
When rotating my scene, if I had wanted to leave the axes as they were and just rotate the cubes, I would move my block of code transforming the model matrix from before the axes are drawn to after the axes are drawn. 