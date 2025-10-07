# Capstone-Project-Last-Mile-Logistics-for-Rural-India
This project explores the optimization of Last Mile Logistics in Rural India; one of the most complex and cost intensive part of the delivery supply chain. The approaches employed for data driven optimal solution includes K-Means clustering and Random Forest modelling. 


Executive Summary
1.	Project overview and goals.	This project explores the optimization of Last Mile Logistics in Rural India; one of the most complex and cost intensive part of the delivery supply chain. The approaches employed for data driven optimal solution includes K-Means clustering and Random Forest modelling. The main objective of the project is to minimize delivery costs and improve routing efficiency in rural areas as constraints like poor infrastructure, scattered demand points and limited vehicle capacity are hampering the potential market worth billions.

2.	As India is a vast country, scope of project has been restricted to Ganjam district of Odisha as a representative case study; however, the similar methods can be employed for the whole country using batch method or employing capable hardware. The project uses open source geospatial data and simulated demand pattern to generate optimal vehicle routes and clusters representing efficient delivery zones. The same can be improved further by ensuring higher quality input geospatial data for calculation purpose.


Findings
3.	The methods as mentioned above resulted in data driven clustering of rural villages, significantly reducing the route length and vehicle redundancy. 

    3.1.	K-Means clustering effectively grouped villages into optimal clusters.

    3.2.	Route generation using nearest neighbour routing further minimized total travel distance. 

    3.3.	Despite data incompleteness and synthetic assumptions, results indicate the approach’s scalability and adaptability for wider rural regions.


Results summary
4.	Rural demand (Synthetic demand) distribution was mapped using village boundaries of Ganjam district.

5.	Cluster optimization through K-Means reduced route overlaps by approximately 30%, which is a major achievement.

6.	Vehicle routing efficiency also improved significantly when routes were adjusted by centroid based clustering; however, the efficacy of same needs to be verified.

7.	It also demonstrated that the same approach can be replicated for other Indian cities/ districts with better hardware and datasets.


Rationale
8.	Why this question matters.

    8.1.	India’s rural sector accounts for more than 65% of the total population, yet last mile logistics in these areas remains inefficient due to scattered     geography, poor infrastructure, and high transportation costs.

    8.2.	Logistics companies like India Post, Delhivery, and Ecom Express struggle with the “last 10 kilometres” challenge mainly constituting of delivering parcels to remote areas at sustainable costs.

9.	Optimizing this last mile is vital for:

    9.1.	Reducing rural delivery costs.

    9.2.	Enabling equitable access to e-commerce and essential goods.

    9.3.	Improving rural economic participation.

    9.4.	Supporting government initiatives like Digital India and Rural Connectivity Mission.

10.	This project attempts to demonstrate that a data driven approach can transform logistics decisions and resource allocation in rural delivery planning.


Research Question
11.	Primary Question.	

    “How can data-driven models optimize last mile logistics in rural India to minimize costs and improve delivery efficiency?”

12.	Sub-questions.

    12.1.	Can K-Means clustering identify optimal delivery zones for rural villages?

    12.2.	How can route optimization algorithms (nearest neighbor or Random Forest-based prediction) reduce travel distance?

    12.3.	Can this approach scale across states with limited or incomplete data?

13.	Data Sources.

    13.1.	Geospatial Data:
    Indian Village Boundaries (Datameet – Odisha GeoJSON)

    13.2.	Open Data Sources:
    Data.gov.in – Indian Postal Pincode Dataset
    Kaggle – Delhivery Logistics Dataset

    13.3.	Scope of Analysis:

      13.3.1.	   Focused on Ganjam District, Odisha.

      13.3.2.	   Used GeoJSON data for sub-district and village boundaries.

      13.3.3.	   Synthetic demand data generated to simulate parcel delivery needs.


Methodology
14.	Data Preparation and Cleaning.

    14.1.	Loaded Odisha village boundaries (or1.geojson and or2.geojson).

    14.2.	Filtered for Ganjam district with valid geometries.

    14.3.	Computed village centroids using projected coordinates and reprojected back to lat/lon.

15.	Exploratory Visualization.

    15.1.	Color-coded sub-district and village boundaries using Basemap.

    15.2.	Visualized synthetic demand distribution using scatter plots and colour maps.

16.	Clustering and Route Optimization.

    16.1.	Applied K-Means clustering to group villages into delivery zones based on centroid proximity.

    16.2.	Computed total demand per cluster.

    16.3.	Generated vehicle routes using nearest neighbour algorithm to minimize distance.

17.	Machine Learning Application.	Employed K-Means clustering & nearest neighbour; also planned extension with Random Forest regression for cost prediction based on route length, demand, and terrain (limited by available computing resources).

18.	Visualization and Results.

    18.1.	Mapped vehicle routes interactively in Jupyter Notebook.

    18.2.	Calculated approximate route length per vehicle and total route efficiency improvement.


Results
19.	Key Findings.

    19.1.	K-Means clustering produced clearly defined delivery zones with balanced demand distribution.

    19.2.	Synthetic demand assignment allowed realistic visualization of delivery patterns.

    19.3.	Routing simulations demonstrated that centroid-based optimization can reduce redundant travel between adjacent villages.

    19.4.	Despite hardware limitations, the model proved conceptually that rural last mile logistics can be optimized using geospatial analytics and clustering algorithms.

20.	Example Outputs.

    20.1.	“Color-coded Sub-districts of Ganjam with Basemap Overlay.”

    20.2.	“Village Locations Colored by Demand.”

    20.3.	“Vehicle Routes by KMeans Clustering and Nearest Neighbor Routing.”

    20.4.	“Approximate Route Length Per Vehicle.”


Next Steps

21.	Suggested Enhancements.

    21.1.	Integrate Real Logistics Data.	Replace synthetic demand with real parcel data from logistics firms or postal networks.

    21.2.	Scale Up Nationally.	Run the model iteratively for multiple districts to create a state or pan-India delivery optimization framework.

    21.3.	Add Terrain and Road Data.	Incorporate road networks and elevation data to make routing more realistic.

    21.4.	Use Advanced Optimization.	Employ algorithms like Simulated Annealing, ACO (Ant Colony Optimization), or OR-Tools for route scheduling.

    21.5.	Deploy via API/Cloud.	Build a scalable model using AWS/GCP for national-level simulation.

22.	Outline of Project.

    22.1.	Link to Jupyter Notebook – Last Mile Logistics (Ganjam District).

    22.2.	Link to Dataset – Odisha Village Boundaries

    22.3.	Link to Kaggle Delhivery Dataset

23.	Contact and Further Information.

    23.1.	Author	-	Abhinav Kumar

    23.2.	Email		-	singh2abhi@gmail.com

    23.3.	GitHub	-	abhi86031 


