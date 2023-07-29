# Traffic-Optimization

## To-do

- Node Map
- Model Clarification
- Set up Thursday meeting

## Explanation

Imagine a map of stations drawn as nodes, and the edges being connections between nodes. Ignoring distance, every node is connected to the others.

Now, imagine that traffic is unevenly split, say 50 cars/hour for a 5 lane road and 0 cars/hour for a 2 lane road that both connect to one node. To balance the traffic, we can reallocate the traffic to have 35 cars/hour on the 5 lane road (7 cars/lane per hour) and then 15 cars/hour on the 2 lane road (7.5 cars/lane per hour). This way, traffic is evened out on every road.

To apply this to an entire region, the traffic volume at each node would then equally distributed to every node (per traffic direction), until the traffic is sufficently redistributed throught the network.

Currently, this program algorithm is very intensive in its recursive resource use, and a more innovative and efficent approach needs to be designed.

## Flows and Flow IDs

Flow IDs are the unique identifier for a flow. Each flow has its own ID, and each flow ID has its own flow. Flows are the traffic flow of a road, and are represented as a list of numbers.

For example, a 3 lane road going in a certain direction is specificed by the road number, the direction, and the lane number. The flow ID would be the road number, the direction, and the lane number. The flow would be the traffic flow of that lane+direction. For example, that road has 6 flows.

## A bit of context

I’ve compiled and attached some articles for research and attached the files for the 2021 January Data and the 2021 Station Data.

- “Traffic flow optimisation in presence of vehicle automation and communication systems – Part I: A first-order multi-lane model for motorway traffic” describes a first-order model created to simulate motorway traffic that is then used in the companion paper.
- “Traffic flow optimisation in presence of vehicle automation and communication systems – Part II: Optimal control for multi-lane motorways” describes an optimal control model that utilizes the previously established motorway model to control on-ramp flow, mainstream flow, and lane changing.
- The files in 2021 January Data represents the traffic flow of all stations in states for certain days to the hour
- The files in 2021 Station Data represents the total traffic flow of all stations in the year along with # of lanes and more location information.

## Information required for model per station

- Station ID (has direction)
- Traffic volume
- Lane count
