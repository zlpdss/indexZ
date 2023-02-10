# indexZ

This is the public layer of indexZ a lightweight level 7 roblox exploit, it allows freedom to developers by even being able to run popular exploits like 
Owlhub, Dex Explorer, and Remote Spy. The exploit can easily use just about every single script in just about every game!

Currently you are not able to join the indexZ development team.

# Download

[Download indexZ](https://github.com/zlpdss/indexZ/blob/main/indexZ.zip)

# Documentation
#### Details
indexZ - 1.2

indexZ nativly runs off of C# however the code editor itself uses Lua, later down the road we will add cross comaptiability 
between the two languages. This does not buffer indexZ's usage in any way though.

**Lua Environments :**

set_fps_cap(int)
Set a custom FPS limit. The game engine's default is 60.

hookfunction((function)old, (function)hook) -
Hooks function 'old', replacing it with the function 'hook'. The old function is returned.

**Mouse Functions -**

MouseMoveRel(int x, int y)	
Moves mouse cursor x pixels left/right and y pixels up/down from the current position.

Aliases: mousemoverel, MouseMoveRelative, mousemoverelative
MouseScroll(int y)	
Simulates mouse to scroll up/down by y pixels.

Aliases: mousescroll
MouseButton1Click()	
Sends left button click signal.

MouseButton1Press()	
Sends left mouse button down signal.

MouseButton1Release()	
Sends left mouse button up signal.

MouseButton2Click()	
Sends right button click signal.

MouseButton2Press()	
Sends right mouse button down signal.

MouseButton2Release()	
Sends right mouse button up signal.

**Console Functions:**

rconsoleprint(string text)	
Opens a console which displays the specified text plainly.

rconsolewarn(string text)	
Opens a console which displays the specified text as a warning.

rconsoleerr(string text)
Opens a console which displays the specified text as an error.

rconsolename(string text)	
Sets the name

Drawing Library Functions :

**Drawing Canvas -**

Drawing.new(string ClassName)	Creates a new Drawing object based on the given class name and returns it.
Drawing.clear()	Clears the Drawing canvas.

**Drawing Classes -**

*Base* - All Drawing classes inherit these properties and functions.

bool Visible
int ZIndex
void Remove()

*Line*

Vector2 From
Vector2 To
Color3 Color
float Thickness
float Transparency

*Text*

string Text
Vector2 Position
float Size
Color3 Color
bool Center
bool Outline
float Transparency
Vector2 TextBounds [readonly]

*Square*

Vector2 Position
Vector2 Size
Color3 Color
float Thickness
bool Filled
float Transparency

*Circle*

Vector2 Position
float Radius
Color3 Color
float Thickness
bool Filled
float Transparency
int NumSides

*Triangle*

Vector2 PointA
Vector2 PointB
Vector2 PointC
Color3 Color
float Thickness
bool Filled
float Transparency

**Example :**

    newSquare = Drawing.new("Square")
    newSquare.Position = Vector2.new(0,0)
    newSquare.Size = Vector2.new(50,50)
    newSquare.Color = Color3.new(0, 1, 0)
    newSquare.Thickness = 16
    newSquare.Rounding = 0
    newSquare.Filled = true
    newSquare.Transparency = 0.5

**Remade RLua Functions :**

game:HttpGet(string url)	
Fetches text from the given URL. game:HttpGet() wraps this so there is URL bypass.
