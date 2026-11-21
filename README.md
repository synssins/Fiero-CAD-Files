# Fiero CAD Files

Shared CAD for the Pontiac Fiero GT: body panels, glass, lights and the steel space frame, in one model. Work in progress, open for contributions.

![Side profile](images/1988%20Fiero%20GT%20Side%20Profile.png)

| | |
|---|---|
| ![Nose](images/1988%20Fiero%20GT%20NoseJob.png) | ![Rear](images/1988%20Fiero%20GT%20DatAss.png) |
| ![With wing](images/1988%20Fiero%20GT%20WingedBeauty.png) | ![Without wing](images/1988%20Fiero%20GT%20Wingless.png) |

![Quarter windows](images/1988%20Fiero%20GT%20Quarter%20Windows.png)

## Layout

| Folder | What is in it |
|---|---|
| `fusion/` | Native Fusion archives (`.f3d`; designs with linked components export as `.f3z`). Keeps the parametric timeline. |
| `step/` | STEP files, for anyone on other CAD software. The full model is at the top; `body/`, `glass/` and `lights/` are for individual component exports. |
| `previews/` | STL copies so GitHub shows a 3D preview in the browser, in the same `body/`, `glass/`, `lights/` layout. Not for editing. |
| `images/` | Screenshots and renders. |

## The model

`fusion/Fiero CAD Model 88 GT v3.f3d` and `step/Fiero CAD Model 88 GT v3.step` are the same model: the full car as separate named components.

- **Body:** nose, hood, front fenders, doors, roof skin, quarter panels and trim, quarter window frames, rear clip, decklid, wing, rear bumper, fuel door, headlight doors, engine vents, moulding.
- **Glass:** rear window, quarter windows.
- **Lights:** tail lights with lenses and masks, brake, turn and reverse lamps, marker lamps.
- **Structure and interior:** space frame, seats.

Units are millimetres. X is width with +X the driver's (left) side, Y is length with the front of the car at -Y, Z is up.

Body panels are 3 mm thick, thickened inward, with the outer surface at the vehicle dimension. They do not yet have the inner mounting flanges the real panels use to bolt to the frame. The space frame is modelled from the B pillars back; the front is not done.

## Contributing

- Keep the units and axes above so parts land in place.
- Put native files in `fusion/`, a STEP export in the matching `step/` subfolder, and an STL in the matching `previews/` subfolder.
- Say where your dimensions came from (measured part, drawing, scan, estimate) in the pull request.
- Corrections from people who have the car apart are the most useful thing you can send.

Large CAD files are stored with Git LFS. Install it once before cloning:

```
git lfs install
git clone https://github.com/synssins/Fiero-CAD-Files.git
```

## License

CC BY 4.0. See `LICENSE`.
