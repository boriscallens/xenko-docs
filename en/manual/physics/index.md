# Physics

![Physics in Xenko](media/physics-index-physics-in-xenko.png)

Xenko simulates real-world physics such as gravity and collisions. This section explains how physics components work, how to add them to your project, and how to use them with scripts.

## In this section

* [Colliders](colliders.md): Create physics by adding collider components to entities
    * [Static colliders](static-colliders.md): Colliders that don't move
    * [Rigid bodies](rigid-bodies.md): Moving objects, affected by gravity and collisions
    * [Kinematic rigid bodies](kinematic-rigid-bodies.md): Physics objects controlled by scripts
    * [Characters](characters.md): Colliders for characters (such as player characters and NPCs)
    * [Collider shapes](collider-shapes.md): Define the shape of collider components
    * [Triggers](triggers.md): Use triggers to detect passing objects
    * [Constraints](constraints.md): Create appealing and realistic physics
* [Raycasting](raycasting.md): Trace intersecting objects
* [Simulation](simulation.md): How Xenko controls physics

### Tutorials

* [Create a bouncing ball](create-a-bouncing-ball.md): Use the static collider and rigid body components to create a ball bouncing on a floor
* [Script a trigger](script-a-trigger.md): Create a trigger that doubles the size of a ball when the ball passes through it

## Further reference

Xenko uses the open-source [Bullet Physics](http://bulletphysics.org/wordpress/) engine. For detailed information, see the [Bullet User Manual](https://github.com/bulletphysics/bullet3/blob/master/docs/Bullet_User_Manual.pdf).