# SpriteFont

The @'SiliconStudio.Xenko.Graphics.SpriteFont' class is a convenient way to draw text. It works with the @'SiliconStudio.Xenko.Graphics.SpriteBatch' class.

>[!Note]
>Remember that you need to put all custom code in a [Custom scene renderer](../graphics-compositor/custom-scene-renderers.md) to include it in the composition.

## Load a spriteFont

After a font asset is compiled it can be loaded as a @'SiliconStudio.Xenko.Graphics.SpriteFont' instance using the @'SiliconStudio.Core.Serialization.Assets.ContentManager'. It contains all the options to display a text (bitmaps, kerning, line spacing etc).

**Code:** Load a SpriteFont

```cs
var myFont = Content.Load<SpriteFont>("MyFont");
```

## Write text on screen

Once the font is loaded, you can display any text with a @'SiliconStudio.Xenko.Graphics.SpriteBatch'. The @'SiliconStudio.Xenko.Graphics.SpriteBatch.DrawString' method performs the draw. For more information about the SpriteBatch, see the [SpriteBatch](spritebatch.md) page.

**Code:** Write text

```cs
// create the SpriteBatch
var spriteBatch = new SpriteBatch(GraphicsDevice);

// don't forget the begin
spriteBatch.Begin(GraphicsContext);
 
// draw the text "Helloworld!" in red from the center of the screen
spriteBatch.DrawString(myFont, "Helloworld!", new Vector2(0.5, 0.5), Color.Red);
 
// don't forget the end
spriteBatch.End();
```

The various overloads let you specify the text's orientation, scale, depth, origin, etc. You can also apply some @'SiliconStudio.Xenko.Graphics.SpriteEffects' to the text:

- None
- FlipHorizontally
- FlipVertically
- FlipBoth

**Code:** Advanced text drawing

```cs
// draw the text "Hello world!" upside-down in red from the center of the screen
spriteBatch.DrawString(myFont, "Hello world!", new Vector2(0.5, 0.5), Color.Red, 0, new Vector2(0, 0), new Vector2(1,1), SpriteEffects.FlipVertically, 0);
```

## See also

* [SpriteBatch](spritebatch.md)