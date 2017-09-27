# Platforms

![Platforms](media/game-engine-system-requirements-intro-pic.png)

Xenko is cross-platform game engine. This means you can create your game once, then compile and deploy it on all the platforms Xenko supports. The engine converts C# and shaders to the different native languages, and abstracts the concepts that differ between platforms, so you don't have to adapt your code for each platform.

## Supported platforms

* Windows Desktop 7, 8, 10
* Windows Universal (UWP)
* [Linux (Ubuntu)](linux/index.md)
* Android 2.3 and later
* iOS 8.0 and later

> [!TIP]
> To check which platform your project uses, add a break point to your code (eg in a script), run the project, and check the [Platform.Type](xref:SiliconStudio.Core.Platform.Type) variable.

## Supported graphics platforms

* DirectX 9 (limited support), 10, 11, 12
* OpenGL 3, 4
* OpenGL ES 2, 3
* Vulkan

>[!Note]
>Xenko only supports MSAA (multisample anti-aliasing) for DirectX 11 and later.
>Xenko's performance with OpenGL ES 2 depends on your device's OpenGL driver (specifically its shader compiler).

>[!Warning]
>DirectX 9 doesn't support HDR textures. Using HDR textures with DirextX 9 will crash your game.

## Set the graphics platform

You set the graphics platform in the **Game settings** asset under **Rendering settings > Target graphics platform**.

![Select graphics platform](media/change-graphics-platform.png)

For more information, see [Set the graphics platform](set-the-graphics-platform.md).

## Preprocessor variables

Xenko defines preprocessor variables if you want to write code that compiles only under a specific platform. For more information, see [Preprocessor variables](../scripts/preprocessor-variables.md).

## In this section

* [Linux](linux/index.md)
* [UWP](uwp/index.md)
    * [Xbox Live](uwp/xbox-live.md)
* [Add or remove a platform](add-or-remove-a-platform.md)
* [Set the graphics platform](set-the-graphics-platform.md)
* [Game settings](../game-studio/game-settings.md).