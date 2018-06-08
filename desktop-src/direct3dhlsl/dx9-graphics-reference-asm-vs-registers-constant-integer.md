---
title: Constant Integer Register
description: Constant integer registers are used only by loop - vs and rep - vs.
ms.assetid: da9916d4-655b-4c98-99a4-1abfa66459b5
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Constant Integer Register

Constant integer registers are used only by [loop - vs](loop---vs.md) and [rep - vs](rep---vs.md).

They can be set using [defi - vs](defi---vs.md) or [**SetVertexShaderConstantI**](https://msdn.microsoft.com/library/windows/desktop/bb174468).

When used as an argument to the [loop - vs](loop---vs.md) instruction:

-   .x is the iteration count. ([rep - vs](rep---vs.md) uses only this component).
-   .y is the initial value for the loop counter.
-   .z is the increment step for the loop counter.

The behavior of shader constants has changed between Direct3D 8 and Direct3D 9.

-   For Direct3D 9, constants set with defx assign values to the shader constant space. The lifetime of a constant declared with defx is confined to the execution of that shader only. Conversely, constants set using the APIs SetXXXShaderConstantX initialize constants in global space. Constants in global space are not copied to local space (visible to the shader) until SetxxxShaderConstants is called.
-   For Direct3D 8, constants set with defx or the APIs both assign values to the shader constant space. Each time the shader is executed, the constants are used by the current shader regardless of the technique used to set them.

## Related topics

<dl> <dt>

[Vertex Shader Registers](dx9-graphics-reference-asm-vs-registers.md)
</dt> </dl>

 

 



