# Vehicle Spec Interaction

## Objective
Build a responsive, interactive UI component for an e-learning course that organizes technical vehicle specifications through progressive disclosure and supports active learner discovery.

## 1. Visual Design & Context

**Course Cohesion:** Inspect the sample components provided in the repository. Your deliverable should match the visual aesthetic (colors, typography, container styling, and spacing) so it blends in with the repository.

**Assets Provided:**
* `truck-image.jpg` — Vehicle image to display upfront.
* `truck-info.jpeg` — Structural layout guide showing content hierarchy and data points.
* `short-info.png` —  The information to be displayed upfront (highlighted in red).

## 2. Interaction Requirements

You must build two states of the component:

### State 1: Overview (Module Start)
**Goal:** Introduce the vehicle without overwhelming the learner with raw data.

**Behavior:**
* Display high-level essential information upfront (the vehicle image and shortened model name).
* Provide an intuitive mechanism to expand, open, or explore deeper technical specifications on demand while maintaining a clean initial footprint.

### State 2: Targeted Task (Active Discovery / Lookup)
**Goal:** Prompt the learner to locate a specific data point—in this scenario, the Engine Type.

**Methodology:**
* **Active Exploration:** Do not auto-expand or immediately hand the answer to the learner. The interface should prompt them to interact and actively locate where that specification lives within the component's structure.
* **Visual feedback:** When the learner successfully identifies or navigates to the correct data point, the component should provide clear visual feedback (e.g., highlighting or confirming the selection).
* **Scaffolding:** The design should accommodate learners who struggle to locate the item by providing intuitive feedback or discoverable guidance rather than dead-ends.

## 3. Technical Notes

* Implement your solution directly within this folder.
* Ensure both State 1 (Overview) and State 2 (Targeted Discovery) can be easily viewed and tested.
* Ensure interactive elements are keyboard-accessible and functional on desktop and tablet viewports.
* Push your work and send an email saying that you've completed the task.