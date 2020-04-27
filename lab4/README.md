Lab 4

24 a) **What is the formula given a u value of the uv coordinate (a value between 0 and 1), I get the x value of the pixel to sample from in this 8x8 texture?**
u * 8(u * textureWidth)

b) **What is the formula given a v value of the uv coordinate (a value between 0 and 1), I get the y value of the pixel to sample from in this 8x8 texture?**
v * 8(v * textureHeight)

c) **What color is sampled from the texture at the uv coordinate (0.375, 0.25)? (sample from the image based on the number your formula gives you i.e. (1, 0) is blue)**
(0.375, 0.25) is white


Cube to the left and in the middle were made through the instuctions we were giving

Cube to the right was made the same just with a new texture/ normal map combo

Cube to the top had its textures loaded with shaders

Cube to the bottom was also loaded with shaders but tiled so the texture is displayed 4x on each side

This was done by multiplying the UV texture space in the vertex shader by 2 which shrinks the uv coordinate system by 1/2 making the texture only cover 1/4 of the cubes surface. Then, inorder to fill in the blanks, I used mod (vUv,1.0)in the fragment shader.

Video: https://drive.google.com/open?id=12qD7vrKlzR_dAsZmsQ9bGn2Xo6D77sWv
