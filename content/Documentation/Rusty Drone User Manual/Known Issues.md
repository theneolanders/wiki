[[- User Manual Info -]]

Default suit size is too small
New busters are positioned wrong in suit mode
Non-trusted pilots can't open their own chest compartment
The chest compartment can't be opened while shutdown, preventing the power core from being reinserted in case of energy loss
Leg raycasts don't account for user scale
Feet don't reposition while inactive, causing them to fly in when deploying or landing
Headguns tilt incorrectly if the drone's head is not facing the same direction as the body
Deploying the minigun too quickly after closing it causes it to have too many barrels
The minigun sound driving doesn’t spool down correctly when retracting
Drone reacts to RustyTalkingLights variable while shutdown
Bitbot doesn't disappear quickly enough during rocket/bike/compact mode transformations
Spawning a tether module sometimes causes a world crash for unknown reasons
Dequipping suit mode doesn't reset hands
Gunshift indicator slides in from the wrong place when the visuals turn on and is very shaky due to async writing

Sequence breaks:
- Turret mode doesn't mesh well with rocket/bike mode
    
- Many features fail to deactivate on shutdown
    
- Switching to bike mode directly from rocket mode while the minigun is deployed will not retract it