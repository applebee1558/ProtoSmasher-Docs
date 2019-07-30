# Classes

## Base
Side note: every class inherits functions and properties from this class.
- bool Visible
- int ZIndex
- void Remove()

## Line
- Vector2 From
- Vector2 To
- Color3 Color
- float Thickness
- float Transparency

## Text
- string Text
- Vector2 Position
- float Size
- Color3 Color
- bool Center
- bool Outline
- float Transparency
- Vector2 TextBounds [readonly]

## Square
- Vector2 Position
- Vector2 Size
- Color3 Color
- float Thickness
- bool Filled
- float Transparency

## Circle
- Vector2 Position
- float Radius
- Color3 Color
- float Thickness
- bool Filled
- float Transparency
- int NumSides

## Triangle
- Vector2 PointA
- Vector2 PointB
- Vector2 PointC
- Color3 Color
- float Thickness
- bool Filled
- float Transparency

## Image
- string Uri
- Vector2 Position
- Vector2 Size [readonly]
- bool Loaded
- float Transparency
- float ScaleFactor (this will update the Size property to reflect the scaled size)