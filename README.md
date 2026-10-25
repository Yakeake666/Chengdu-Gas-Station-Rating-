# Oil Review Map 
A location-based gas station review application powered by real driver feedback. In China, different gas station provide oil with different qualities. Oil with low quality damages engines and reduces the life of engines. To avoid this problem, I made this app, allowing drivers to rate each gas station. Therefore, drivers can choose the stations that provide better oil.
## Features
1. Interactive Map Homepage: Full-screen map browsing with a top floating search bar (by name or address) and multi-dimensional filter chips (brand, rating, distance).

2. Dynamic Status Icons: Map markers feature dynamic colored rings (green, yellow, red) based on the station's overall rating for instant visual feedback.

3. Quick Bottom Sheet: Tapping a map marker smoothly slides up a key info card (station name, distance, overall rating) with a direct link to the details page.

4. Multi-Dimensional Rating Panel: Separates "Service Attitude" and "Fuel Quality" scores, moving beyond generic single-star ratings.

5. Interactive Rating Controls: A dual 5-star rating system with dynamic text prompts (ranging from "Terrible" to "Excellent"), supporting detailed text reviews and submission validation.

6. User Profile & Growth System: A centralized hub displaying the user's published reviews, received likes, and account settings.

##  Map Engine & Data Source

Currently, this repository uses a **simulated placeholder map** built with Flutter's native widgets (`Stack` and `Container`). This design allows you to clone, run, and test the UI immediately without needing to configure complex API keys or billing accounts.

For production and **real-time map rendering**, this application is designed to seamlessly integrate with commercial Map SDKs. To display live maps, real-time traffic, and accurate GPS positioning, you will need to register for a developer account and plug in your preferred engine:

*   **Global Users:** [Google Maps Flutter](https://pub.dev/packages/google_maps_flutter) (Recommended for international geolocation, real-time routing, and Places API).
*   **Mainland China Users:** [AMap (高德地图) SDK](https://pub.dev/packages/amap_flutter_map) or [Baidu Map SDK](https://pub.dev/packages/baidu_map_flutter) (Highly recommended for accurate local gas station POI data and domestic navigation).
*   **Open Source Alternative:** [flutter_map](https://pub.dev/packages/flutter_map) paired with Mapbox or OpenStreetMap (OSM) tile servers.

*Note: Real-time gas station coordinates (POI data), live fuel prices, and dynamic routing will need to be fetched via your backend using the Web APIs provided by your chosen map engine.*
