# Flutter Lab: Expanded, Flexible, and Flex Ratios

In this lab, you will learn how to make your UI responsive. You will explore the difference between the `Expanded` and `Flexible` widgets, and learn how to distribute space proportionally using the `flex` property.

## Core Concepts
- **`Expanded`**: Forces the child widget to stretch and fill all available extra space. (Tight fit).
- **`Flexible`**: Allows the child widget to take up extra space, but doesn't *force* it to stretch if it has its own size. (Loose fit).
- **`flex` property**: When multiple widgets are expanding, this number tells Flutter how to divide the space. If you have two widgets, one with `flex: 1` and one with `flex: 2`, the screen is divided into 3 total parts (1 + 2). The first widget gets 1 part, and the second gets 2 parts (making it twice as large).

## Prerequisites
1. Clone this repository to your local machine.
2. Run `flutter pub get` in your terminal.
3. Launch an emulator or connect a physical device, and run the app. 

## Instructions
Open `lib/main.dart` and locate the `TODO` comments. 

1. **Test Expanded**: Go to `TODO 1` and wrap the cyan container in an `Expanded` widget. Notice how it ignores its own width and stretches to push the grey boxes to the edges.
2. **Test Flexible**: Go to `TODO 2` and wrap the pink container in a `Flexible` widget. Notice how it stays exactly 120 pixels wide instead of stretching.
3. **Test Flex Ratios**: Go to `TODO 3`, `4`, and `5`. Wrap all three colored containers in `Expanded` widgets. Give the outer two containers `flex: 1`, and the middle purple container `flex: 2`. 

## Expected Output
When completed, your screen will show three rows:
1. A Row with a stretched cyan box in the middle.
2. A Row with a compact pink box in the middle.
3. A Row filled end-to-end with color, where the purple box in the middle is exactly twice as wide as the amber and green boxes on the sides!
