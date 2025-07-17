## Projects

### 1. [Agentic Resume Generator](https://resume-updater-one.vercel.app/)
 I built this because I was changing and updating my resume very frequently and formatting it correctlty after even small changes was turning out to be a very time-consuming task. So I built a full-stack web application that acts as an intelligent assistant to automate the tedious process of editing and reformatting resumes. By simply giving natural lamguage commands such as 'add my project as an AI engineer where I completed the following work...', you can get properly formatted resume bullet points in LaTeX and an Overleaf document.

- Engineered an AI Agent by integrating the Google Gemini API with a Node.js backend to intelligently parse and act on natural language commands
- Developed a  prompt engineering strategy to convert unstructured resume text and user commands into a strictly-typed JSON object, enabling reliable and predictable modifications
- Built a custom function to parse the resume and convert it into a string that can be passed into the prompt
- Automated the creation of LaTeX documents by building a server-side generator that converts the JSON into "Jake's Resume" format
- Designed and built a minimalist UI from scratch using React and custom CSS
- Streamlined the final compilation step by integrating a direct "Open in Overleaf" feature, which POSTs the generated .tex code into a new project for immediate PDF viewing and download

### 2. [Coffee dialing-in assistant](https://coffee-dial-in.vercel.app/)
For any coffee enthusiast,'dialing in' — the process of finding the perfect grind size for a specific combination of coffee beans, grinder, and brew method is a frustrating and wasteful cycle of trial and error. I created the AI Coffee Assistant to solve this problem. It replaces hours of manual research with a single, intelligent query. By leveraging a generative AI (Google Gemini API) with real-time web access, the application acts as an expert barista on demand. It automates the entire research and synthesis process, delivering a tailored, evidence-based starting point in seconds. 

- Architected and built a full-stack application using a React/Vite/Tailwind CSS frontend and a Node.js/Express backend, establishing a secure client-server model to protect sensitive API credentials.
- Implemented an advanced Retrieval-Augmented Generation (RAG) workflow by integrating the Google Gemini Pro API. The system performs live, targeted web searches to analyze real-time data, overcoming the limitations of static models.
- Engineered a sophisticated prompt strategy that instructs the AI to act as a domain expert, evaluate conflicting web sources, and return structured JSON for seamless and reliable frontend integration.
- Developed a dynamic and responsive user interface focused on a clean, intuitive experience, managing asynchronous state to provide users with real-time feedback and data-driven results.

### 3. [TritonMates – Full-Stack Roommate Management App](https://github.com/a2jensen/CSE-110-TritonMates)
- Built a full-stack web app on Next.js + Tailwind CSS for the frontend and Firebase for backend functionalities.
- Incorporated Firebase Auth for secure Google sign-in, facilitating seamless user and data storage in Firestore.
- Adopted Agile methodologies for iterative development, conducting sprint reviews and integrating user feedback.
- Utilized GitHub for version control, managing feature development, issue tracking and debugging effectively.

### 4. [User Rating Prediction Recommender System and Research Paper](https://drive.google.com/file/d/1jTe1jFSHnlCgZ76BHsqI3kpLeLlQJZ5O/view?usp=drive_link)
- Conducted exploratory data analysis on a Food.com recipe and review dataset, identifying skews and key insights to guide predictive modeling.
- Pre-processed data by handling missing values, filtering sparse reviews and users, and ensuring data validity for robust predictions.
- Implemented Word2Vec similarity and SVD latent factor models to predict user ratings, optimizing hyperparameters and applying regularization to improve performance.
- Evaluated models using MSE, MAE, and RMSE, identified scalability challenges, and proposed future improvements based on comparisons with similar projects.

### 5. Web Developer
- Developed sticky note web application using React, enabling users to create, edit, delete, and filter notes, utilizing the useState hook for real-time state management.
- Implemented a to-do list app using React, allowing users to add tasks, mark them as completed, and dynamically update the UI based on user actions, improving task management efficiency.
- Integrated favorites toggle functionality in the sticky note app, providing users the ability to mark notes as important or remove them from the list, with seamless state transitions through React hooks.
- Built responsive web applications with interactive features such as filtering notes based on user input, enhancing the user experience by leveraging React's component-based architecture.
- Managed state across multiple components using useState, optimizing the performance and functionality of the web apps to improve user interaction and responsiveness.

### 6. Huffman Encoding Tree for File Compression
- Built a Huffman encoding tree to perform file compression and decompression on file headers
- Implemented a file compression tool using the Huffman algorithm to reduce storage size without losing information
- Implemented a file decompression tool using the Huffman algorithm to get back the original file header
- Used a priority queue to further make the process more efficient
- Enhanced the efficiency of the compression by using bit-packing (3-bit integers) to store larger numbers in smaller sequences

### 7. Graph Class and Algorithms Implementation
- Implemented important graph algorithms to represent and analyze network
- Developed a Graph class to represent undirected graphs, applied to transmission clustering for HIV and COVID-19
- Utilized the graph to identify transmission clusters and gather information for virus spread prevention through graph
algorithms using BFS, Djikstra’s Algorithm, Connected Components, and Connecting Thresholds
