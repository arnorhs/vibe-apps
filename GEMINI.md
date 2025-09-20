This repository, `vibe-apps`, serves as a collection of single-page web applications, each residing in its own subdirectory under `apps/`. The project is configured to serve these applications using `http-server`.

Currently, the repository contains two distinct applications:

### 1. NetPlug (apps/netplug/index.html)
**Description:** NetPlug is a "Home Network Planner" tool. It provides a visual canvas where users can design and plan their home network layouts.
**Features:**
- **Device Management:** Users can add pre-defined network devices (e.g., Unify Cloud Gateway, Zyxel Switch, Unify Access Point, Server, ISP Gateway) to the canvas.
- **Custom Devices:** The application allows for the creation of custom devices, where users can specify the device name and the number of LAN and SFP+ ports.
- **Interactive Canvas:** Devices can be dragged and dropped around the canvas.
- **Cable Drawing:** Users can draw virtual cables between the ports of different devices to represent network connections.
- **Text Labels:** The ability to add and position text labels on the canvas for annotations.
- **Canvas Panning:** The canvas can be panned to navigate larger network layouts.
- **Search Functionality:** A search box to quickly find and add devices from the available database.
- **Reset Option:** A button to clear the canvas and start a new plan.
**Technology Stack:** The application is built as a single HTML file, leveraging Tailwind CSS for styling and vanilla JavaScript for all interactive functionalities.

### 2. Reps Maker (apps/repsmaker/index.html)
**Description:** Reps Maker is a personal workout program builder. It enables users to create and track their exercise routines.
**Features:**
- **Exercise Set Creation:** Users can define custom exercise sets, each with a unique name and a list of exercises.
- **Exercise Details:** Each exercise within a set can have a name and an optional URL (presumably for reference or demonstration videos).
- **Local Storage Persistence:** Exercise sets and workout records are saved to the browser's local storage, allowing users to retain their data across sessions.
- **Workout Recording:** For any saved exercise set, users can initiate a "Record Workout" session. This displays a grid showing each exercise, the data from the previous workout (if available), and an input field to log the current workout's details (e.g., "3x10 @ 135lbs").
- **Workout Saving:** The current workout data can be saved, updating the "previous workout" record for future sessions.
**Technology Stack:** This application is also a single HTML file, using basic CSS for styling and vanilla JavaScript for all its logic and data management.

The project's `package.json` indicates the use of `http-server` for serving the `apps` directory, `prettier` for code formatting, and `typescript` with `vite` in `devDependencies`, suggesting potential for future development or a build process not currently applied to the existing single-file apps.