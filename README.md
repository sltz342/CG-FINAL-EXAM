This repo serves as my submission for Intro to Computer Graphics Final Exam, for the year of 2024, Fall Semester.

I implimented the following Shaders for my Mario Kart Practical.

Color Vertex Shader. Outline Shader. Rainbow Wave Shader. Toon Shader

![{2B5493A7-6804-4612-BF18-6E5E800AEBBF}](https://github.com/user-attachments/assets/4671a8d2-8d24-4410-bc7f-c6265977b7ea) ![{EA08606B-4F0B-4830-A5B6-5B31BD5E5538}](https://github.com/user-attachments/assets/19ff712c-3310-4535-9676-dec2016eb9ee) ![{CBE20B88-10B6-4FA5-AE88-F991F64D9296}](https://github.com/user-attachments/assets/30aa5524-7420-49b7-b3a0-39f7dbeeff8f) ![{AAF04BCC-8E05-4146-AB0B-AC1769265458}](https://github.com/user-attachments/assets/52ec7a64-1ce0-475a-b627-edeebbd2b71a)


Color Vertex Shader:

This shader was implemented via HSL and focus on changing the colors of a vertex via the screen space posistions as opposed to a normal shader using the world space posistions.
Depending on where the shader is in relation to the camera, verts closer to the top left turn green while verts closer to the bottom right turn red.
![{53A030B3-431D-440F-9A0B-3264F2A64CCC}](https://github.com/user-attachments/assets/8bfcf01c-854a-4533-b6bd-2c8896cc14dc) ![{CBBD6C06-6F63-4AD7-A1E8-C4161CD59159}](https://github.com/user-attachments/assets/00b3e5e4-8a88-4cb4-8576-9dc8c1e6cd8d)

I choose to use a Color Vertex Shader for the stands of the map because I wanted an interesting effect that would be interesting to look at and would change it's color depending on where you were when you started looking at it. 
![Blank diagram](https://github.com/user-attachments/assets/af00ca9a-6d5e-491c-ab2f-73872a9b191f)





Outline Shader:

I Wanted the Player to stand out from the everchanging wave rainbow texture that was on the floor, so I gave them an outline shader in order to make them more visible and pop out.
I achieved this by creating a shader that would cull verts if they were determined to be in front of the camera, by using screen space projection and the normals of the verts. If the verts normals' were facing away from the camera, they were not culled. 
![{0D377DF9-A52B-4A90-9042-9676C63E64A6}](https://github.com/user-attachments/assets/02c6de46-ea51-4d89-9e5e-974327d49571)

Rainbow Wave Shader:
I wanted the ground to be similar to the original image for Super Mario Kart with Rainbow Ride being a rainbow road in space. As such, I created a wave effect that would combine two different rainbow textures to create a shimmering and moving rainbow effect on the ground, which looks better than the originals' static material for the road.


https://github.com/user-attachments/assets/2e3434d3-d628-403a-a636-a1505a0bb6dc


