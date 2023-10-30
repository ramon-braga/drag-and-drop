# Drag and Drop Project Overview

This project offers a simple drag and drop experience, allowing users to rearrange numbered pieces into a correct sequence within designated areas. Successful arrangement is indicated by a color change in the target areas.

## Technical Details

The project is primarily built using HTML, CSS, and JavaScript. Here's a breakdown of the key components:

- **index.html:** This file establishes the main structure of the project.
- **assets/:** This folder contains the necessary style and script files.
- **script.js:** This file manages the drag and drop functionality within the project.
- **style.css:** This file defines the visual appearance of the project.

## Functionality

### Drag and Drop

Users can drag numbered pieces from the initial area to any of the three target areas. Target areas are highlighted when ready to receive the piece.

- `dragStart`: Initiates the dragging process by assigning a 'dragging' class to the moving piece.
- `dragEnd`: Ends the dragging process and removes the 'dragging' class from the piece.

### Target Areas

These are the designated areas where pieces can be dropped.

- `dragOver`: Allows a piece to be dropped in an empty target area.
- `dragLeave`: Removes visual highlighting from the target area when the piece is dragged away.
- `drop`: Places the piece in the target area if it's empty and updates the area information accordingly.

### Neutral Area

The neutral area serves as the initial location for the pieces, enabling users to return pieces to their original positions.

- `dragOverNeutral`: Allows the piece to be dropped back into the neutral area.
- `dragLeaveNeutral`: Removes the visual highlight from the neutral area when the piece is moved away.
- `dropNeutral`: Returns the piece to the neutral area and updates the area information.

### Game Logic

The `updateAreas` function manages the state of the areas based on the current arrangement of the pieces. If all areas contain the numbers 1, 2, and 3 respectively, the 'correct' class is added to the areas section.

## Usage

- Open the [link](https://ramon-braga.github.io/drag-and-drop/).
- Drag the numbered pieces into the target areas.
- Arrange the pieces in the correct sequence (1, 2, 3) within the target areas.
