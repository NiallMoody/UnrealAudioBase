# Unreal Audio Base
![Editor screenshot of the project](https://raw.githubusercontent.com/NiallMoody/UnrealAudioBase/main/Docs/Screenshot.jpg)

This project was created as a base for students to explore audio implementation in Unreal. I currently use it in labs for my **CMP407: Audio Programming** module at [Abertay University](https://www.abertay.ac.uk/).

Developed in **Unreal 5.4.3**.

As it is intended as a base for audio implementation, it features the following:

- Different surfaces to walk on/in (concrete, grass, water)
- Different shapes and sizes of enclosed spaces (with expectations of their own acoustic characteristics, i.e. reverb)
- Unreal's default third-person model for timeline-based footstep triggering
- A small variety of buttons and triggers
- A small pool of water for experimenting with sonic underwater effects

Note that the 'puzzles' are not particularly challenging. This may change in future, see the [ToDo list](https://github.com/NiallMoody/UnrealAudioBase/blob/main/ToDo.md).

# Additional notes about the project
As it's a third-person game, most materials make use of a masking shader that will cut out geometry around the player character so that the player has a clearer view of the level.

This makes it a little difficult to edit the level/geometry in the editor, so it is disabled (`0.0`) by default. It can be enabled (`1.0`) via the **MPC_Masking_Toggle** Material Parameter Collection:

![Screenshot of the location of MPC_Masking_Toggle](https://raw.githubusercontent.com/NiallMoody/UnrealAudioBase/main/Docs/MaskingToggleLocation.png)
