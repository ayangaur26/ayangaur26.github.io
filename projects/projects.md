## Projects

### 1. [Autonomous Driving GEM e4](https://github.com/ansh1113/gem_vlm_navigation)
*Python, PyTorch, ROS, SLAM, LiDAR, GPT-4o | Jan 2026 – May 2026*
- Integrated GPT-4o multimodal reasoning into a VLM navigation stack for natural language-commanded driving
- Engineered LiDAR/stereo perception and factor-graph SLAM pipeline, halving trajectory ATE RMSE to 0.34m
- Developed a CenterPoint 3D detector and AB3DMOT tracker using Kalman filtering for multi-class inference
- Implemented an A* planner and Stanley controller to achieve 0.09m cross-track error across 25 real-world paths
- Deployed stack to hardware via PACMod, publishing 20 Hz control commands across ROS 1 and ROS 2

### 2. Autonomous Bipedal Robot
*C++, ESP32, FreeRTOS, I2C, PID | Jan 2026 – May 2026*
- Developed ESP32 C++ firmware using FreeRTOS for real-time task scheduling and hardware timer configuration
- Implemented low-level I2C drivers for IMU, OLED, and I/O expanders with safe shared-bus access
- Architected control stacks with Kalman filtering for attitude estimation and PID for PWM motor actuation
- Designed autonomous navigation featuring waypoint planners and UDP over Wi-Fi ground station telemetry

### 3. Autonomous IoT Robot Car & Embedded Navigation Stack
*Raspberry Pi, Python, OpenCV, TFLite, A*, Custom PCB | Jan 2026 – Present*
- Designed and routed a custom 2-layer PCB (Gerber layout) interfacing Raspberry Pi GPIO, DC motor drivers, grayscale module, photo-interrupters, and battery power.
- Implemented dual-layer computer vision on Picamera2: real-time OpenCV HSV color masking for traffic rule compliance (Red STOP sign detection and halt) and TensorFlow Lite (TFLite EfficientDet-Lite) for COCO person detection.
- Built a 1 cm resolution Cartesian occupancy grid mapping engine using stationary servo-panned (40°–140°) ultrasonic sensor sweeps with obstacle clearance inflation.
- Developed an A* path planning algorithm with 4-connected grid graph traversal and Manhattan heuristic for cardinal 90° leg navigation, dynamic re-sweeping, and real-time obstacle avoidance replanning.
- Calibrated motor PWM timing and dead-reckoning pose tracking with cell tolerance thresholding to eliminate goal overshoot without encoders, integrating a live map/camera dashboard over SSH tunnels.

### 4. AI Email Agent
As a student and aspiring software engineer, I found that managing job and internship applications was a chaotic and manual process. Tracking the status of dozens of applications, from initial submission to interview requests and rejections, meant juggling countless emails and manually updating spreadsheets. I knew that this repetitive, error-prone workflow was a perfect candidate for automation. I built an AI Email Agent to ease this burden, creating a centralized, intelligent system to manage the entire process with ease.

- Utilized LangChain to orchestrate a sequence of NLP tasks with a Large Language Model (Groq/Ollama). This pipeline performed email classification, named entity extraction (company, role), intent analysis (application status), and context-aware text generation for drafting replies.
- Built a robust backend with Node.js, Prisma, and PostgreSQL that uses the Gmail threadId as a unique key. This ensures data idempotency by intelligently updating existing application records from email replies rather than creating duplicate entries.
- Integrated multiple Google Workspace APIs (Gmail, Sheets) through a secure OAuth 2.0 flow. The system manages access tokens and granular permission scopes to programmatically read email threads, create drafts, and append data to spreadsheets on the user's behalf.
- Built a responsive, client-style user interface in React and TypeScript. Managed complex asynchronous state with useEffect hooks to orchestrate chained API calls, fetching and displaying application lists from the database, live email threads from Gmail, and AI-generated drafts in a seamless user experience.

### 5. [Agentic Resume Generator](https://resume-updater-one.vercel.app/)
 I built this because I was changing and updating my resume very frequently and formatting it correctlty after even small changes was turning out to be a very time-consuming task. So I built a full-stack web application that acts as an intelligent assistant to automate the tedious process of editing and reformatting resumes. By simply giving natural language commands such as 'add my project as an AI engineer where I completed the following work...', you can get properly formatted resume bullet points in LaTeX and an Overleaf document.

- Engineered an AI Agent by integrating the Google Gemini API with a Node.js backend to intelligently parse and act on natural language commands
- Developed a  prompt engineering strategy to convert unstructured resume text and user commands into a strictly-typed JSON object, enabling reliable and predictable modifications
- Built a custom function to parse the resume and convert it into a string that can be passed into the prompt
- Automated the creation of LaTeX documents by building a server-side generator that converts the JSON into "Jake's Resume" format
- Designed and built a minimalist UI from scratch using React and custom CSS
- Streamlined the final compilation step by integrating a direct "Open in Overleaf" feature, which POSTs the generated .tex code into a new project for immediate PDF viewing and download

### 6. STM32 - BLE Tracker Device
- Programmed device drivers for GPIO and built an accelerometer abstraction enabling motion detection
- Implemented privacy-enabled BLE functionality to broadcast status, from device only when lost
- Minimized current draw from 1800µA-30µA through sleep mode and interrupt-based accelerometer handling

### 7. [Coffee dialing-in assistant](https://coffee-dial-in.vercel.app/)
For any coffee enthusiast, 'dialing in' — the process of finding the perfect grind size for a specific combination of coffee beans, grinder, and brew method is a frustrating and wasteful cycle of trial and error. I created the AI Coffee Assistant to solve this problem. It replaces hours of manual research with a single, intelligent query. By leveraging a generative AI (Google Gemini API) with real-time web access, the application acts as an expert barista on demand. It automates the entire research and synthesis process, delivering a tailored, evidence-based starting point in seconds. 

- Architected and built a full-stack application using a React/Vite/Tailwind CSS frontend and a Node.js/Express backend, establishing a secure client-server model to protect sensitive API credentials.
- Implemented an advanced Retrieval-Augmented Generation (RAG) workflow by integrating the Google Gemini Pro API. The system performs live, targeted web searches to analyze real-time data, overcoming the limitations of static models.
- Engineered a sophisticated prompt strategy that instructs the AI to act as a domain expert, evaluate conflicting web sources, and return structured JSON for seamless and reliable frontend integration.
- Developed a dynamic and responsive user interface focused on a clean, intuitive experience, managing asynchronous state to provide users with real-time feedback and data-driven results.

### 8. [TritonMates – Full-Stack Roommate Management App](https://github.com/a2jensen/CSE-110-TritonMates)
- Built a full-stack web app on Next.js + Tailwind CSS for the frontend and Firebase for backend functionalities.
- Incorporated Firebase Auth for secure Google sign-in, facilitating seamless user and data storage in Firestore.
- Adopted Agile methodologies for iterative development, conducting sprint reviews and integrating user feedback.
- Utilized GitHub for version control, managing feature development, issue tracking and debugging effectively.

### 9. [User Rating Prediction Recommender System and Research Paper](https://drive.google.com/file/d/1jTe1jFSHnlCgZ76BHsqI3kpLeLlQJZ5O/view?usp=drive_link)
- Conducted exploratory data analysis on a Food.com recipe and review dataset, identifying skews and key insights to guide predictive modeling.
- Pre-processed data by handling missing values, filtering sparse reviews and users, and ensuring data validity for robust predictions.
- Implemented Word2Vec similarity and SVD latent factor models to predict user ratings, optimizing hyperparameters and applying regularization to improve performance.
- Evaluated models using MSE, MAE, and RMSE, identified scalability challenges, and proposed future improvements based on comparisons with similar projects.

### 10. Web Developer
- Developed sticky note web application using React, enabling users to create, edit, delete, and filter notes, utilizing the useState hook for real-time state management.
- Implemented a to-do list app using React, allowing users to add tasks, mark them as completed, and dynamically update the UI based on user actions, improving task management efficiency.
- Integrated favorites toggle functionality in the sticky note app, providing users the ability to mark notes as important or remove them from the list, with seamless state transitions through React hooks.
- Built responsive web applications with interactive features such as filtering notes based on user input, enhancing the user experience by leveraging React's component-based architecture.
- Managed state across multiple components using useState, optimizing the performance and functionality of the web apps to improve user interaction and responsiveness.

### 11. Huffman Encoding Tree for File Compression
- Built a Huffman encoding tree to perform file compression and decompression on file headers
- Implemented a file compression tool using the Huffman algorithm to reduce storage size without losing information
- Implemented a file decompression tool using the Huffman algorithm to get back the original file header
- Used a priority queue to further make the process more efficient
- Enhanced the efficiency of the compression by using bit-packing (3-bit integers) to store larger numbers in smaller sequences

### 12. Graph Class and Algorithms Implementation
- Implemented important graph algorithms to represent and analyze network
- Developed a Graph class to represent undirected graphs, applied to transmission clustering for HIV and COVID-19
- Utilized the graph to identify transmission clusters and gather information for virus spread prevention through graph
algorithms using BFS, Djikstra’s Algorithm, Connected Components, and Connecting Thresholds
