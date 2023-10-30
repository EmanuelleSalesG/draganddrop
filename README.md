# Drag and Drop Project
## Overview
This is a simple drag and drop project where you can move numbered pieces into one of three areas below to arrange them in the correct sequence. 
The order in which you release the object matters. If the player gets the sequence right, the area will turn green to indicate success.

## How it Works
The project is built using HTML, CSS, and JavaScript. Here's a brief explanation of the code:

- `index.html`: This is the main file containing the HTML structure of the project.
- `assets/`: This folder contains the style and script files.
- `script.js`: This file contains the JavaScript code that controls the drag and drop behavior.
- `style.css`: This file contains the styling code for the project's appearance.

## Functionality
### Drag and Drop
Numbered pieces can be dragged from the initial area to one of three target areas. The target areas will change color to indicate they are ready to receive the piece.

- dragStart: Initiates the dragging process. The piece being dragged gets a dragging class.
- dragEnd: Ends the dragging process. The dragging class is removed from the piece.

### Target Areas
The target areas are the three areas where pieces can be dropped.

- dragOver: Allows the piece to be dropped in the target area if it's empty.
- dragLeave: Removes the visual highlight from the target area when the piece is dragged out.
- drop: Places the piece in the target area if it's empty and updates the information about the areas.

### Neutral Area
- The neutral area is the initial area where the pieces are located. It allows moving pieces back to the original position.
- dragOverNeutral: Allows the piece to be dropped in the neutral area.
- dragLeaveNeutral: Removes the visual highlight from the neutral area when the piece is dragged out.
- dropNeutral: Places the piece back in the neutral area and updates the information about the areas.

### Game Logic
The updateAreas function is responsible for updating the state of the areas based on the current arrangement of the pieces. If all areas are correct (containing the numbers 1, 2, and 3 respectively), the correct class is added to the areas section.

### How to Use
Open the [link]()
Drag the numbered pieces to the target areas.
Try to get the correct sequence (1, 2, 3) in the target areas.
