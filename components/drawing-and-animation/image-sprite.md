# Image Sprite

A rectangular 'sprite' that can be placed on a Canvas, where it can react to touches and drags, interact with other sprites (ImageSprites and other Balls) and the edge of the Canvas, and move according to its property values.

For example, to have an ImageSprite move 4 pixels toward the top of a Canvas every 500 milliseconds (half second), you would set the Speed property to 4 [pixels], the Interval property to 500 [milliseconds], the Heading property to 90 [degrees], and the Enabled property to True. These and its other properties can be changed at any time.

The difference between a Ball and an ImageSprite is that the latter can get its appearance from an image file, while a Ball's appearance can only be changed by varying its PaintColor and Radius properties.

---

### Properties

#### Enabled

Controls whether the sprite moves when its speed is non-zero.

#### Heading

Returns the sprite's heading in degrees above the positive x-axis. Zero degrees is toward the right of the screen; 90 degrees is toward the top of the screen.

#### Interval

The interval in milliseconds at which the sprite's position is updated. For example, if the interval is 50 and the speed is 10, then the sprite will move 10 pixels every 50 milliseconds.

#### Speed

The speed at which the sprite moves. The sprite moves this many pixels every interval.

#### Visible

True if the sprite is visible.

#### X

The horizontal coordinate of the left edge of the sprite, increasing as the sprite moves to the right.

#### Y

The vertical coordinate of the top of the sprite, increasing as the sprite moves down.

#### Z

How the sprite should be layered relative to other sprits, with higher-numbered layers in front of lower-numbered layers.

---

### Events

#### CollidedWith(component other)

Handler for CollidedWith events, called when two sprites collide. Note that checking for collisions with a rotated ImageSprite currently checks against the sprite's unrotated position. Therefore, collision checking will be inaccurate for tall narrow or short wide sprites that are rotated.

#### Dragged(number startX, number startY, number prevX, number prevY, number currentX, number currentY)

Handler for Dragged events. On all calls, the starting coordinates are where the screen was first touched, and the "current" coordinates describe the endpoint of the current line segment. On the first call within a given drag, the "previous" coordinates are the same as the starting coordinates; subsequently, they are the "current" coordinates from the prior call. Note that the Sprite won't actually move anywhere in response to the Dragged event unless MoveTo is specifically called.

#### EdgeReached(number edge)

Event handler called when the sprite reaches an edge of the screen. If Bounce is then called with that edge, the sprite will appear to bounce off of the edge it reached. Edge here is represented as an integer that indicates one of eight directions north(1), northeast(2), east(3), southeast(4), south (-1), southwest(-2), west(-3), and northwest(-4).

#### Flung(number x, number y, number speed, number heading, number xvel, number yvel)

When a fling gesture (quick swipe) is made on the sprite: provides the (x,y) position of the start of the fling, relative to the upper left of the canvas. Also provides the speed (pixels per millisecond) and heading (0-360 degrees) of the fling, as well as the x velocity and y velocity components of the fling's vector.

#### NoLongerCollidingWith(component other)

Event indicating that a pair of sprites are no longer colliding.

#### TouchDown(number x, number y)

When the user begins touching the sprite (places finger on sprite and leaves it there): provides the (x,y) position of the touch, relative to the upper left of the canvas

#### TouchUp(number x, number y)

When the user stops touching the sprite (lifts finger after a TouchDown event): provides the (x,y) position of the touch, relative to the upper left of the canvas

#### Touched(number x, number y)

When the user touches the sprite and then immediately lifts finger: provides the (x,y) position of the touch, relative to the upper left of the canvas

Methods

---

#### Bounce(number edge)

Makes this sprite bounce, as if off a wall. For normal bouncing, the edge argument should be the one returned by EdgeReached.

#### boolean CollidingWith(component other)

Indicates whether a collision has been registered between this sprite and the passed sprite.

#### MoveIntoBounds()

Moves the sprite back in bounds if part of it extends out of bounds, having no effect otherwise. If the sprite is too wide to fit on the canvas, this aligns the left side of the sprite with the left side of the canvas. If the sprite is too tall to fit on the canvas, this aligns the top side of the sprite with the top side of the canvas.

#### MoveTo(number x, number y)

Moves the sprite so that its left top corner is at the specfied x and y coordinates.

#### PointInDirection(number x, number y)

Turns the sprite to point towards the point with coordinates as (x, y).

#### PointTowards(component target)

Turns the sprite to point towards a designated target sprite. The new heading will be parallel to the line joining the centerpoints of the two sprites.
