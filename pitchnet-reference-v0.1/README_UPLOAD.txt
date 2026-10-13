PitchNet Reference Vocal v0.1 - changed files

Goal of this build:
- Add File > Load Reference Vocal...
- Analyze the reference with a separate EditorController / Project
- Display reference notes and pitch curve as a read-only grey ghost overlay
- Keep the editable target vocal unchanged
- Build as "PitchNet Dev" so it can coexist with the normal PitchNet build

Files to replace in your GitHub fork:
.github/workflows/dev-windows.yml
Source/UI/Commands.h
Source/UI/Main/MenuHandler.cpp
Source/UI/MainComponent.h
Source/UI/MainComponent.cpp
Source/UI/Main/MainComponent_ProjectIO.cpp
Source/UI/PianoRollComponent.h
Source/UI/PianoRollComponent.cpp

This is milestone 1 only. It does NOT yet implement one-note Fit to Reference.
After successful build and reference overlay verification, the next milestone is:
1) select one target note
2) select one reference note
3) Fit to Reference: timing + pitch + pitch curve
