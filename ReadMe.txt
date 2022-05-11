Evan Sinasac - 1081418
INFO6020 Graphics 2

Built and run in Visual Studio Community Debug and Release x64

CONTROLS
WASD			- Move camera
QE			- Raise/lower camera
Space			- Set view position (meant to be like a security camera or something)
B			- Turn debug objects on
M			- Change all models to wireframe
Keypad 1-6		- Change FBO resolution
P			- Set FBO resolution to current window size
1-9			- Different Offscreen 2D Effects
0			- Clear Offscreen 2D Effects

FRAGMENT SHADER
I really only made changes to the fragment shader, specifically to continue using the DFK models and textures, and to implement the different 2D effects.  I added a "twoDEffectOperator" that determines what kind of effect is being applied at any time, these are changed by using the number keys 1-9.  For the Skybox Reflect and Refract I added them to my "textureOperator" statement, so if the model itself has the textureOperator set to 5 or 6, that model will reflect/refract the skybox.  Did not implement dynamic environment.  Had to modify the light pass for the DFK models to use the normal map, the calcualteLightContrib already handles the ambient occlusion for the DFK models.

MODELS
The models I used are from Runemark's Dark Fantasy Kit (https://assetstore.unity.com/packages/3d/environments/fantasy/dark-fantasy-kit-123894) and some of the other models given to us from class/exams.

TEXTURES
I am using the textures from Runemark's Dark Fantasy Kit that go with the respective objects I converted, as well as some other textures we were give in class.  All textures are found in the textures folder, the Scope and Window were just quick Google searches for something to try the offscreen mask.


Video Demo: https://youtu.be/waFB7Q75Ny8