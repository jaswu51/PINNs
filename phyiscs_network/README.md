### Translation/Rotation physics, inertia computation

https://www.youtube.com/watch?v=DCfIofZ6BY8

### Kinematics Of Rigid Bodies - General Plane Motion

https://www.youtube.com/watch?v=4LsLy9iJKFA

### Definite intervals

https://www.youtube.com/watch?v=-JSVueLK3fc

### Friction detection, yes in Isaac Sim and no in Mujoco

Isaac Sim provides the capability to sense friction during simulation. Friction is an important physical property that affects the interaction and movement of objects in a simulated environment. Here's a general overview of how friction can be sensed in Isaac Sim:

Material properties: In Isaac Sim, friction is typically defined through material properties assigned to objects. Each object or surface in the simulation can be assigned a specific material with predefined friction coefficients. Friction coefficients determine the amount of resistance or friction that occurs when objects slide or interact with each other.

Physics simulation: Isaac Sim employs the NVIDIA PhysX physics engine, which simulates the physical behavior of objects. PhysX takes into account the friction coefficients of materials to calculate the forces and torques acting on objects during collisions, contacts, and movements.

Contact sensing: Isaac Sim provides contact sensing capabilities to detect and measure contact forces between objects. When objects come into contact or collide, contact sensors can capture the resulting forces, including friction forces. These contact forces can be used to estimate the friction between surfaces or objects.

Force and torque sensors: Isaac Sim allows the attachment of force and torque sensors to objects. These sensors can measure the forces and torques acting on an object during interactions, including frictional forces. By attaching such sensors to objects involved in frictional interactions, you can obtain direct measurements of friction forces.

By utilizing the physics simulation capabilities and contact sensing features in Isaac Sim, you can effectively sense and analyze friction forces between objects. This information can be used for various purposes, such as evaluating the performance of robot grippers, optimizing motion planning algorithms, or developing controllers that account for frictional effects.

In the MuJoCo (Multi-Joint Dynamics with Contact) physics engine, friction detection is not a direct feature provided by the engine itself. MuJoCo focuses on efficient simulation of rigid body dynamics and contact interactions, but it does not have built-in capabilities specifically dedicated to friction detection or estimation.

However, MuJoCo does provide access to contact forces and torques between objects during simulation. By analyzing these contact forces, you can infer the presence and effects of friction to some extent. Frictional forces arise as a result of contact interactions, and the magnitude and direction of these forces can give you an indication of the friction present in the simulation.

To detect or estimate friction using MuJoCo, you would typically need to implement your own algorithms or techniques. This could involve analyzing the contact forces, applying friction models, or using custom sensor measurements to estimate frictional effects.

It's worth noting that MuJoCo is a highly customizable physics engine, and it provides an extensive API that allows users to implement their own sensors and controllers. With the flexibility offered by MuJoCo, you can design and integrate custom sensors that specifically capture and measure frictional forces within your simulations.

Overall, while MuJoCo does not offer direct friction detection functionality out of the box, it provides the tools and capabilities necessary to analyze and estimate friction forces based on contact interactions and custom sensor measurements.

### Bias Force

Bias force refers to an additional force acting on an object or system that can affect its motion. In the context of Coriolis, centrifugal, and gravitational forces, bias forces are associated with specific physical phenomena.

Coriolis Force: The Coriolis force is an apparent force that acts on a moving object in a rotating frame of reference. It arises due to the rotation of the Earth and is perpendicular to both the velocity of the moving object and the axis of rotation. The Coriolis force influences the direction of motion of objects, causing them to deflect to the right in the Northern Hemisphere and to the left in the Southern Hemisphere. This force is responsible for phenomena like the rotation of weather systems and the deflection of moving objects on the Earth's surface.

Centrifugal Force: The centrifugal force is a fictitious or pseudo force that appears to act on an object moving in a rotating frame of reference. It is directed away from the center of rotation and is proportional to the distance of the object from the axis of rotation. The centrifugal force arises due to inertia and is perceived as an outward force. In reality, it is not a true force but rather an effect observed in a rotating reference frame. The centrifugal force plays a role in various systems, such as the behavior of objects in rotating machinery or the dynamics of particles in a centrifuge.

Gravitational Force: The gravitational force is the force of attraction between two objects with mass. It is one of the fundamental forces of nature and is responsible for holding celestial bodies like planets, stars, and galaxies together. The gravitational force follows the inverse-square law, which means it weakens with distance. In the context of bias forces, gravitational force can introduce a bias in the motion of objects, particularly when dealing with systems affected by gravity, such as satellites orbiting a planet or a spacecraft undergoing gravitational maneuvers.

In summary, bias forces such as Coriolis, centrifugal, and gravitational forces are additional forces that can influence the motion of objects or systems in specific contexts, and their effects need to be considered when analyzing or predicting motion in those scenarios.
