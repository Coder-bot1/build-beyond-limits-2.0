Project Name:
Open Viking

Attendee/Team Details:
Name: Syed Ali Naimath Muqashif GitHub Username: Coder-bot1 LinkedIn Profile: https://www.linkedin.com/in/syed-ali-naimath-muqashif-4a197a36b/
Name: Mohd Kareem Uddin GitHub Username: KareemAshh LinkedIn Profile: https://www.linkedin.com/in/mohd-kareem-uddin-baaa70276?
Name: Syed Mohammed Aqheel GitHub Username: Aqheel65 LinkedIn Profile: https://www.linkedin.com/in/syed-mohd-aqheel-34a326357
Name: Syed Zeeshan Mehdi GitHub Username: zeeshan-rgb LinkedIn Profile: https://www.linkedin.com/in/syed-zeeshan-3abaa9331/

Problem Statement Selected
OpenViking
Choose one:
Problem statement 2

Project Description:
VikingMind is a context-aware developer assistant dashboard designed to visualize how AI agents retrieve codebase context via OpenViking and optimize database queries using **Valkey** (a high-speed, Redis-compatible key-value cache).
* What is the project about?
It is a real-time developer interface and simulation console demonstrating context-aware RAG trajectory tracing and cache optimization.
* Who is it for?
AI application developers, system architects, and engineers building autonomous agentic coding assistants.
* What problem does it solve?
RAG (Retrieval-Augmented Generation) pipelines are often black boxes. Developers cannot easily see how context is retrieved, what queries hit/miss the cache, or how latency behaves.
* How does it help the user?
It provides instant visibility into prompt retrieval paths and Valkey cache metrics, allowing developer teams to debug, profile, and optimize AI context-retrieval pipelines.

Approach:
1. User Experience Design: Created a responsive, premium three-panel dashboard layout (Workspace File Explorer on the left, Conversational AI Chat in the middle, and Retrieval Trajectory/Valkey Monitoring on the right).
2. Visual Trajectory Tracing: Modeled a tree/step visualizer to show exactly how a user query gets parsed, checked against Valkey cache, run through semantic/vector search, re-ranked, and finally injected into the LLM context.
3. Simulated Live Metrics: Designed interactive charts tracking key Valkey metrics (Hit/Miss ratio, CPU/Memory load, query latency) in real-time, especially under simulated heavy traffic.
4. Clean Web Architecture: Developed using modern glassmorphism styling and vanilla web components (HTML/CSS/JS) to make the MVP extremely fast, lightweight, and easy to run without heavy build toolchains.

Tech Stack and Tools Used:
Frontend: HTML5, Vanilla CSS (Premium Glassmorphism Design System), Vanilla JavaScript (ES6)
Backend: Python (Simple HTTP Server for local hosting)
Database: Valkey / Redis-compatible cache (Simulated/Mocked dashboard endpoints)
AI Tools/API: OpenViking context engine (Simulated trajectory endpoints)
Other Tools: Cursor / Antigravity, Docker, Git

Key Features:
1. Interactive RAG Chat Simulation: Interactive chat panel with preloaded deep-dive developer queries and responses.
2. Visual Retrieval Trajectory Tree: Real-time step-by-step tracing of OpenViking context search paths.
3. Valkey Cache Metrics Dashboard: Real-time status display and performance charts showing memory usage, latency spikes, and Hit/Miss ratios.
4. Workspace Workspace Navigator: Integrated mock file explorer representation for indexing simulation.

What is Working:
* Premium dark-theme glassmorphism UI with smooth animations and responsive layout.
* Full simulation flow: clicking chat actions triggers simulated Valkey metrics updates and live-drawing retrieval paths.
* Local Python dev server configuration.

What is Still in Progress:
Direct WebSocket or REST API integrations to query a live Docker-based Valkey cache (`localhost:6379`) and a running OpenViking engine backend (`localhost:1933`).

Screenshots or Demo:

Challenges Faced:
* Building responsive graphs and tracing steps dynamically using pure vanilla JS/CSS without using heavy chart libraries like Chart.js or D3.js.
* Designing a premium user experience that visually highlights the concept of cache hits vs. database search latency.

Learnings:
* Gained a deep understanding of OpenViking's RAG context retrieval logic.
* Learned how Valkey behaves as a high-speed caching layer to drastically reduce token usage and context extraction latency.

Future Improvements:
* Integrating real-time metrics pulling using `redis` client connections in a lightweight Node.js/Python backend.
* Adding a file-drop zone to let developers upload real files and watch OpenViking index them in real-time.

