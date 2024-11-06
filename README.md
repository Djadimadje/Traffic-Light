SPECIFICATION (NARRATION) OF GISHUSHU TRAFFIC LIGHTS
The Gishushu Traffic Lights are designed to manage vehicle and pedestrian traffic flow at an intersection, providing safe passage for both vehicles and pedestrians. 
The traffic lights alternate between allowing North-South and East-West traffic, with additional pedestrian crossing states triggered by pedestrian requests.

STATES AND TRANSITIONS

Green Light for North-South Traffic (GreenNS)

Description: The North-South traffic light is green, allowing vehicles in this direction to go.
Duration: 30 seconds.
Transition:
After 30 seconds, transition to the Yellow Light for North-South (YellowNS) state.
Yellow Light for North-South Traffic (YellowNS)

Description: The North-South traffic light turns yellow, indicating that vehicles should prepare to stop.
Duration: 5 seconds.
Transition:
After 5 seconds, transition to the Red Light for North-South (RedNS) state.
Red Light for North-South Traffic (RedNS)

Description: The North-South traffic light is red, stopping all vehicles in this direction.
Duration: 30 seconds if there’s no pedestrian request; otherwise, the duration adjusts based on the pedestrian crossing.
Transitions:
If the pedestrian button is pressed, transition to Pedestrian Crossing.
If no pedestrian request is present and 30 seconds have passed, transition to the Green Light for East-West (GreenEW) state.
Pedestrian Crossing

Description: The pedestrian light flashes to allow pedestrians to cross safely. Vehicles in all directions are stopped.
Duration: 20 seconds.
Transition:
After 20 seconds, transition back to Red Light for North-South (RedNS) if North-South is scheduled next, or Green Light for East-West (GreenEW) if East-West traffic is next.
Green Light for East-West Traffic (GreenEW)

Description: The East-West traffic light is green, allowing vehicles in this direction to go.
Duration: 30 seconds.
Transition:
After 30 seconds, transition to the Yellow Light for East-West (YellowEW) state.
Yellow Light for East-West Traffic (YellowEW)

Description: The East-West traffic light turns yellow, indicating that vehicles should prepare to stop.
Duration: 5 seconds.
Transition:
After 5 seconds, transition to the Red Light for East-West (RedEW) state.
Red Light for East-West Traffic (RedEW)

Description: The East-West traffic light is red, stopping all vehicles in this direction.
Duration: 30 seconds.
Transition:
After 30 seconds, transition back to Green Light for North-South (GreenNS) if North-South traffic is next, or Pedestrian Crossing if a pedestrian request is present.

This setup allows the system to regulate vehicle flow effectively while accommodating pedestrian needs. The sequence also ensures that no direction is given indefinite priority, creating a balanced and safe traffic control system for Gishushu.
