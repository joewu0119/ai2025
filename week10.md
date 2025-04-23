### 1. Materials & Setup

- The “DronePaint” PDF
- Laptops with internet access and ChatGPT
- Shared slide template (3 slides max)


### 2. Reference Questions for Learning

- In two sentences, what is DronePaint?
- How do hand gestures move the drones?
- What is the system archtecture?
- Why do we smooth my hand’s path before flying?
- Three simple metaphors for LightPaint?



🛰️ In two sentences, what is DronePaint?
DronePaint is an interactive system that enables users to control a swarm of drones for light painting using hand gestures recognized by a Deep Neural Network (DNN). The system processes the user’s gestures in real time to generate smooth trajectories that the drones follow to create dynamic light art in midair.

✋ How do hand gestures move the drones?
Hand gestures are recognized using a camera and a DNN-based gesture recognition system that classifies hand poses into predefined commands. These commands are used to draw or erase trajectories, which are then smoothed, processed, and converted into flight paths that the drones follow.

⚙️ What is the system architecture?
DronePaint’s architecture consists of three main modules:

Human-Swarm Interface – captures and interprets hand gestures using a webcam and the Mediapipe framework.

Trajectory Processing Module – smooths and interpolates the drawn paths to generate equidistant points.

Drone Control System – translates processed trajectories into drone movements using the ROS framework and controls the drone swarm with a potential field-based navigation algorithm.

🧹 Why do we smooth my hand’s path before flying?
Smoothing the hand-drawn path ensures that the drone flies along a stable and safe trajectory. It filters out noise and irregular movements to produce equidistant, smooth flight coordinates that help maintain consistent drone motion and avoid erratic behavior.

💡 Three simple metaphors for LightPaint?
Etch A Sketch in the Sky – your hand draws shapes in the air, and the drones trace those patterns with light.

Finger-painting with Fireflies – like waving glowing bugs into patterns that stay suspended in space.

Airbrush for the Night Sky – your gestures become strokes that drones paint with light in three dimensions.
