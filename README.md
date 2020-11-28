# Gooey

An asset module for our beloved gooeys.
It provides the models, materials and textures for both Gooeys and their weird, manic cousins the MawGooeys.

## Gooeys

The Gooey gLTF model can be referenced in prefabs with a `skeletalMesh` as `MawGooey:gooey`.
```json5
  "skeletalMesh": {
    "mesh": "MawGooey:gooey"
  }
```

The model currently comes with one animation only, which is the `ArmatureAction`.
This animation can be referenced in a `skeletalMesh` with an `animationPool` as `MawGooey:gooey#ArmatureAction`.
```json5
  "skeletalMesh": {
    "mesh": "MawGooey:gooey",
    "animationPool": [
      "MawGooey:gooey#ArmatureAction"
    ],
    "loop": true
  }
```

There is a bunch of textures and materials provided that allow for gooeys in many colors of the rainbow.
The materials can be referenced in a `skeletalMesh` as `MawGooey:gooeySkin<color>` with `<color>` being the color name, e.g. "Blue".
```json5
  "skeletalMesh": {
    "mesh": "MawGooey:gooey",
    "material": "MawGooey:gooeySkinBlue"
  }
```

The material and texture assets are named based on the [HTML Color Names](https://htmlcolorcodes.com/color-names/) of the respective color code of the color used in the texture.



## MawGooeys

The MawGooey gLTF model can be referenced in prefabs 

The Gooey gLTF model can be referenced in prefabs with a `skeletalMesh` as `MawGooey:mawgooey`.
```json5
  "skeletalmesh": {
     "mesh": "MawGooey:mawgooey"
   }
```

The model comes with four different animations:
- Attack
- Death
- IdleFinal
- Walk

These animations can be referenced in a `skeletalMesh` with an `animationPool` as `MawGooey:mawgooey#<animation>` with `<animation>` being the animation name, e.g. "Walk".
```json5
  "skeletalMesh": {
    "mesh": "MawGooey:mawgooey",
    "animationPool": [
      "MawGooey:mawgooey#Walk"
    ],
    "loop": true
  }
```

Currently, there are three different color variants provided: Green, Purple, and Red.
The materials can be referenced in a `skeletalMesh` as `MawGooey:mawgooeySkin<color>` with `<color>` being the color name, e.g. "Red".
```json5
  "skeletalMesh": {
    "mesh": "MawGooey:mawgooey",
    "material": "MawGooey:mawgooeySkinRed"
  }
```

The material and texture assets are _not_ aligned with any "official" colors.