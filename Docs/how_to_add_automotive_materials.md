How to add the automotive materials
===================================

CARLA uses Epic Game's Automotive Materials package for a realistic car paint
look. Due to license restrictions we are not allowed to redistribute this
package. In this document we explain how to download and link these materials to
our vehicles.

Download from Marketplace
-------------------------

Epic Games' [Automotive Materials][automatlink] package can be downloaded for
free from the Unreal Engine Marketplace.

NOTE: Unfortunately, Unreal's Marketplace is only available on Windows, so you
need a Windows machine to download this package.

  1. Install Epic Games Launcher from [www.unrealengine.com](https://www.unrealengine.com).
  2. Buy the [Automotive Materials][automatlink] package for $0.
  3. Create a new dummy project and add the Automotive Materials package to it.
  4. Inside the "Content" folder of the newly created project, you can find the "AutomotiveMaterials" folder. Copy this folder to the CARLA project
    - `{NewProject}/Content/AutomotiveMaterials` --> `{CARLA}/Unreal/CarlaUE4/Content/AutomotiveMaterials`

[automatlink]: https://www.unrealengine.com/marketplace/automotive-material-pack

Manually link the materials
---------------------------

Right after opening the project, you should link the automotive materials you
just downloaded.

In the content browser, go to "Content/Static/Vehicles/MaterialRedirectors" and
open "RedirectorInstance".

![Unreal Engine Screenshot 1](img/materials_screenshot_00.png)

Under the "Details" pane, search for the "Parent" material, and replace
"DummyCar" material by "M_Carpaint" material.

![Unreal Engine Screenshot 2](img/materials_screenshot_01.png)

Now save "RedirectorInstance", and you are ready to go.