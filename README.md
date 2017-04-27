# geometry
Packages for common geometric calculations including the ROS transform library, "tf". Also includes ROS bindings for "bullet" physics engine and "kdl" kinematics/dynamics package.

tf2.lookupTransform
tf.waitForTransform

tf has to distinguis between past and future messages

Lookup would require extrapolation into the future.  Requested time 1477388584.595752588 but the latest data is at time 1477388584.587707281, when looking up transform from frame [map_base_link_3_ROI_ORIGIN] to frame [radar_frame]

Lookup would require extrapolation into the past.  Requested time 1477388584.595752588 but the latest data is at time 1477388584.607707281, when looking up transform from frame [map_base_link_3_ROI_ORIGIN] to frame [radar_frame]

Waiting for a message which may arise in the future, or hasn't even arrived yet is worthit.
But if you the latest tf message is already younger than the requested one (extrapolation into the past), it is very unlike "actually" impossible that this data may arrive in the future
