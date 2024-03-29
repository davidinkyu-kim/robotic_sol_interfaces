# Robotic solution interfaces
This package contains message and service definition needed for `robotic_sol` package.

## Messages
* `Sensor3dof.msg`
  - A message for sensor of 3-DOF containing 3 `float64` sensor values.
* `SensorsOutput.msg`
  - A message containing array of multiple sensors. Broadcasted by Node: `robotic_sol/sensor_client_node`.

## Services
* `ReadSensor.srv`
  - A service to obtain sensor values via service call. `sensor_name` is distinguished by the service topic(e.g. `robotic_sol/sensor1/srv/read_sensor`), so request will be empty.
