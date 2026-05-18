# TORCS Lab Results

## Baseline Run (No modifications)
**Parameters used:** All defaults (TARGET_SPEED=100, STEER_GAIN=30, 
CENTERING_GAIN=0.20, BRAKE_THRESHOLD=0.9, ENABLE_TRACTION_CONTROL=True)

**What I observed:**
- Car drove well on the track initially
- Around 02:30, the car got stuck on the wall/grass and lost speed
- The tires seemed to stop working effectively after going off track
- Around 04:00, the car escaped the wall but couldn't regain speed
- Eventually timed out with "Timeout for client answer" errors

**Track:** E-Track 1 (Quick Race)

---

## Task 3: First Modification - Increased Target Speed

**Parameter changed:** TARGET_SPEED = 100 → TARGET_SPEED = 150

**What I observed:**
- Car moved noticeably faster on straight sections
- Struggled more in corners at higher speed
- Went off track more frequently than baseline
- Shows that higher speed requires better steering calibration

**What I learned:**
- Small parameter changes have big effects on behavior
- Speed and stability are a tradeoff
- Real AI engineers face the same balance in autonomous vehicles

## Reflection

**One thing that surprised me:**
- How much a single parameter change affected the car's behavior, just increasing speed made the whole driving style unstable

**One thing I would try next:**
- Adjust STEER_GAIN and BRAKE_THRESHOLD together with higher speed 
to find a better balance between fast and stable driving

**What this taught me about AI:**
- AI systems require constant iteration and tuning during test to find the best plan 
- Simulation is a safe way to experiment before real-world deployment
