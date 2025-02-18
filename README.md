# Expo Camera Preview Freeze on Android

This repository demonstrates a bug in the Expo Camera API where the preview freezes on some Android devices. The issue occurs after extended use or taking multiple pictures. The camera module doesn't throw errors; it simply stops displaying the preview.

## Bug Reproduction

1. Clone this repository.
2. Run the project using Expo Go on a susceptible Android device.
3. Observe the camera preview. After a period of use (varies by device), the preview will freeze.

## Solution

A solution is provided in `cameraBugSolution.js`. This involves adding a timeout to periodically restart the camera. This isn't an ideal solution but it's a workaround until a more robust fix is available from the Expo team.