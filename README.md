# star-network-resilience-rennes| A network-analysis
STAR Transport Network: Analysis, Vulnerabilities & Resilience Strategies in Rennes

This project investigates the structure, vulnerabilities, and resilience of the public transport network in Rennes, France (STAR network), using network science, social network analysis, and propagation modeling techniques.

Through advanced data processing and visual exploration, we aim to:

    Map the transport network as a graph (stops as nodes, connections as edges)

    Analyze structural properties (degree, betweenness, closeness, eigenvector centralities)

    Identify critical hubs and simulate targeted and random disruptions

    Model delay propagation using a network-based SIR-inspired approach

    Provide strategic recommendations to improve robustness and mitigate crisis impacts

Data & Methodology

    Source: GTFS (General Transit Feed Specification) data from STAR Rennes (https://transport.data.gouv.fr/datasets/versions-des-horaires-theoriques-des-lignes-de-bus-et-de-metro-du-reseau-star-au-format-gtfs)

    Processing: Cleaning stop_times, linking source-destination pairs, geospatial enrichment

    Analysis: Centrality metrics, community detection (modularity), network visualization

    Simulation: Delay propagation modeled as temporal spread across the network (SIR logic)

    Tools: R, igraph, ggraph, sf, leaflet, dplyr, and spatial visualizations

Key Insights

    République, Henri Fréville, and Villejean-Université are the most central and vulnerable nodes.

    Random disruptions have minimal impact; targeted attacks fragment the network significantly.

    Stations like Monniais, though less central, are critical due to their influence on accessibility.

    Delay simulations show peak congestion followed by natural dissipation phases.

    Community detection reveals 20 strongly connected clusters aligned with spatial patterns.

Strategic Recommendations

    Reinforce core hubs like République with fallback infrastructure

    Improve redundancy by adding secondary connections between peripheral zones

    Analyze asymmetric routes to ensure bidirectional mobility

    Develop contingency plans targeting key nodes to maintain service continuity

    Use community structures to localize crisis responses during epidemics or major disruptions

Limitations

    The model relies on static GTFS data; real-time mobility and frequency variations are not included

    Propagation dynamics are theoretical and not calibrated against empirical delays

    Socioeconomic constraints and user behavior are not yet modeled

Authors

Gyldano DADJEDJI, Kwami NOUCHET, Ancelin LEBOUDEC
December 11, 2024
