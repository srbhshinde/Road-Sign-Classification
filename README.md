# Road-Sign-Classification
Building digital maps is challenging, and maintaining it up to date in an ever-changing world is even more challenging. Various machine learning techniques helps us to detect road signs and changes in real world, and process it to update maps.

given a sign detected on a road from a 4-camera setting on vehicle, the closest sighting of the sign may be in the right facing camera, with a sharp sign angle with respect to the direction of the car on which cameras set is mounted. Next step for updating map using this sign is to identify the exact road on which this sign is to be placed or applied.

On a + junction, when a sign is detected on the right camera, its hard now to tell if this sign is for the straight road, or for the right-side road, unless you consider parameters like sign bounding box aspect ratio.

For example, a sign detected from Front camera will have a natural aspect ratio of the sign when it is actually facing front of the car, however when same sign is detected on a right-side camera with a sharp angle from front, sign bounding box gets skewed, giving a hint that although its detected in right, it’s still facing the front of the car.

Dataset provided here has details on camera sign was detected, Angle of sign with respect to front in degrees, Sign's reported bounding box aspect ratio (width/height), Sign Width and Height, and the target feature Sign Facing, which is where the sign is actually facing.

Goal here is to predict where the sign is actually facing with respect to the vehicle, given above set of inputs.
