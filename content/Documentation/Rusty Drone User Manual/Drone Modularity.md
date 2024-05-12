[[- User Manual Info -]]

The Rusty Drone utilizes multiple different snapper tags for its modularity functions. The following documentation serves as both a record of these systems and a guide on how to interface with them.
## RustyScreen
The "RustyScreen" tag is used for goggles and glasses, almost always covering the eyes.
## RustyArm
This tag is the most in-depth in terms of required systems to function. Slots with a RustyArm Snapper are to be oriented such that the positive Z-axis is facing away from what it is attached to and positioned such that the origin of the object is the attachment point.
#### Parent Values
RustyArm Snappers can read the following parent values

| Tag         | Data Type | Function                                                                                   |
| ----------- | --------- | ------------------------------------------------------------------------------------------ |
| IsAttached  | Bool      | Signals if the arm is in a valid SnapTarget                                                |
| IsDeployed  | Bool      | If the arm has a retraction state, this controls it                                        |
| IsGrabbable | Bool      | Whether or not the part can be grabbed.                                                    |
| Chirality   | Bool      | Determines chirality of the attached hand (if applicable). True for right, False for left. |
| WristPoint  | Slot      | The slot the onboard IK will attempt to match the position of                              |
| ArmPoint    | Slot      | The slot the onboard IK will point the upper arm at                                        |
## RustyHand
If used, the RustyHand tag should be located on the end of a RustyArm oriented such that the fingers point along the positive Z-axis (this should result in the palm being at the "bottom). The origin of the hand should be positioned at the wrist's pivot point.

| Tag         | Data Type | Function                                                              |
| ----------- | --------- | --------------------------------------------------------------------- |
| IsAttached  | Bool      | Signals if the hand is in a valid SnapTarget                          |
| IsDeployed  | Bool      | If the arm has a retraction state, this controls it                   |
| IsGrabbable | Bool      | Whether or not the part can be grabbed.                               |
| Chirality   | Bool      | Determines chirality (if applicable). True for right, False for left. |
