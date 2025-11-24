[Change Log (2025-11-24):
- Added activity pool size of 3-5 activities per category for more options
- Limited ativities to a distance threshold
- Added fallback rules
- Expanded evening options


Create a short list of candidate activities (3–5 per category such as attractions, restaurants, parks).  
Each activity includes:
- Type (e.g., food, culture, nature)  
- Estimated duration  
- Cost range  
- Distance from lodging or city center  

Fallback rules:  
- If lodging unknown → assume city center.  
- If budget missing → default to mid-range.  
- If interests unspecified → provide a balanced mix (food, culture, nature).  

Use a simple loop to build days:

for each day:  
    pick Morning activity (≤15 min walk or ≤5 km from lodging)  
    pick Midday activity (nearby attraction, same district if possible)  
    pick Afternoon activity (different theme for variety)  
    pick Evening option (restaurant, cultural show, night walk, or casual activity)
