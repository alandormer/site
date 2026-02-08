Site Intelligence Layer — Working Overview
What This Is
Most CCTV and camera systems either record video or trigger basic alerts. On their own,
they provide limited understanding of what is actually happening on a site.
We have built a site intelligence layer that uses computer vision on live camera feeds to
analyse activity locally and convert what happens on site into structured, queryable
operational data.
The system does not stop at detection. Activity is structured, stored, and made usable after
the fact for review, reporting, and oversight.
In practice, this allows organisations to:
●
●
Monitor what activity is happening on a site in real time, and
Review, analyse, and report on what happened later
This is what turns cameras from passive recording devices into a usable site intelligence
layer.
The Core Problem
Existing video systems:
●
●
●
●
●
Detect simple things (person, vehicle, motion)
Push alerts directly to operators
Generate large amounts of noise
Depend on constant human attention
Leave little usable information behind
They tell us:
“What is visible right now?”
They do not tell us:
●
●
●
●
What actually mattered to the user
What changed over time
What is normal for this site
What can be queried
What our Intelligence Layer does
Using the cameras and infrastructure already in place, the system can mirror what CCTV /
camera system providers currently carry out, including
●
●
●
●
●
Monitor activity across sites
Detect presence, movement, access and egress
Track vehicle and pedestrian behaviour
Check safety conditions (e.g. PPE use, zone activity)
Apply consistent rules across camera feeds
What Makes It Different
Most camera‑based AI systems stop at detection or alerts. Our approach separates
observation, recording, and understanding.
Instead of cameras talking directly to humans, the system:
●
●
●
●
●
●
Analyses activity using computer vision at the camera feed
Applies rules and logic consistently across feeds
Converts observations into structured, time‑stamped events
Stores all activity as a factual record
Generate structured reports and documents
Allows operators and managers to query and review activity later
The result is not just live awareness, but a structured record of site activity over time.
What the Platform Delivers
Because all activity is structured and stored, the system can produce:
●
●
●
●
●
Incident and investigation reports
Compliance and audit trails
Shift and daily handovers
Activity summaries and timelines
Evidence for insurance or review
This also enables longer‑term insights, such as:
●
●
●
Pattern detection
Trend analysis
Understanding how a site actually operates day‑to‑day
The key point is that nothing disappears once the moment passes.
Why This Matters
This approach delivers:
●
●
●
●
●
Far less alert noise
Lower operator fatigue
Faster and more reliable incident review
Clear, explainable timelines
Evidence that can be stood over
It allows organisations to move from watching cameras to understanding sites.
Where It’s Used
The system is designed for environments that:
●
●
●
●
Already operate camera networks
Require oversight of physical activity
Need traceability and auditability
Operate in regulated or high‑responsibility contexts
Typical environments include:
●
●
●
●
●
●
Industrial and construction sites
Universities and campuses
Facilities and estates teams
Event venues and temporary sites
Transport and logistics environments
Insurance and risk review teams
Deployment & Data Control
The platform is designed to run:
●
●
●
On‑premise
Local software/models
In private or restricted environments
Key principles:
●
●
●
No mandatory cloud dependency
Full control over data retention and access
Raw data stays where required
This makes the system suitable for regulated, sensitive, or temporary deployments.
How the Intelligence Layer Works
The intelligence layer combines computer vision with structured analysis over time:
●
●
●
●
Computer vision‑based analysis at ingestion
Specialised analysis modules focused on specific questions (e.g. safety, access,
activity patterns)
Pattern detection and comparison over time
Incident summarisation and reporting
Optional agents support interpretation, summarisation, and presentation. All agent outputs
are grounded strictly in recorded observations and stored events.
The system is designed as extensible infrastructure, allowing additional analysis,
interpretation, and reporting capabilities to be added without changing the core event model.
Current State
●
●
●
●
●
Live camera feed ingestion and analysis
Structured event generation
Persistent storage of site activity
Operator‑focused dashboards
Reporting and handover outputs
The system is already running end‑to‑end with live video.
Route to Market & Commercial Direction
The platform is designed to be deployed and delivered primarily through systems
integrators already operating across physical sites and regulated environments.
These include:
– Security and CCTV integrators
– Facilities and estates service providers
– Integrators operating in regulated or data-sovereign environments
This approach allows organisations to add a site intelligence layer to existing camera
deployments without replacing hardware or core systems.
For integrators, it provides a way to offer higher-value intelligence, reporting, and oversight
capabilities on top of existing camera installations.
Technical Architecture — Reference
This section provides a technical reference for how the system is structured and deployed. It
is intended for deeper technical discussion and can be separated into its own document if
required.
Five‑Layer System
1. Observation Layer
●
●
●
●
Camera feeds and video sources (RTSP, files, streams)
Edge‑side processing and frame sampling
Fast local analysis for presence, movement, and basic activity
Produces raw, factual observations
2. Analysis Modules
●
●
●
●
Independent, specialised services
Each module answers a narrow, well‑defined question (e.g. PPE use, access/egress,
spatial change, scene state)
Modules can run concurrently and evolve independently
New modules can be added without changing infrastructure
3. Canonical Events
●
●
●
●
Observations are converted into structured, time‑stamped events
Events are deterministic, normalised, and auditable
Original facts are preserved and never overwritten
Provides a consistent data model across all analyses
4. Event Bus & Storage
●
Central event pipeline for all site activity
●
●
●
All events are stored persistently
Nothing is lost or discarded by default
Enables replay, audit, comparison, and re‑analysis over time
5. Interpretation & Reporting
●
●
●
Operator dashboards and timelines
Reports, summaries, and handover documents
AI‑assisted narratives grounded strictly in recorded events
Data Sovereignty & Deployment Model
The system is designed with data sovereignty as a first‑class concern.
Key principles:
●
All processing can run fully on‑premise or at the edge
●
No mandatory cloud dependency
●
No requirement for external AI services
●
Full control over data retention, access, and deletion
Raw video and derived data remain within the environment defined by the operator. This
makes the system suitable for:
●
●
●
Regulated industries
Public sector deployments
Sensitive or restricted sites
●
Temporary or mobile deployments
Design Principles
●
●
●
●
●
Low noise over high sensitivity
Memory over momentary alerts
Explainability over automation
Modularity over monolithic systems
Facts first, interpretation second
This technical reference supports the core overview above and reflects the current system
architecture.