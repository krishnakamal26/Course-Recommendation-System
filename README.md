Course Recommendation System 🚀
A Dockerized machine learning-based web application that recommends similar courses from a dataset of over 3,000 courses on Coursera. The app uses text vectorization and cosine similarity to provide personalized course recommendations based on user input.

Features 🔥
Data preprocessing and cleaning
Vectorization of course descriptions and skills using sklearn
Cosine similarity-based course recommendation engine
Interactive web interface built with Streamlit
Fully Dockerized for easy deployment
Table of Contents 📑
Installation
Project Structure
Usage
Docker
Contributing
Contact
Installation 🛠️
To run the project locally, follow these steps:

Clone the repository:

git clone https://github.com/ganesh2409/Course-Recommendation-System.git
cd Course-Recommendation-System
Create and activate a virtual environment (optional but recommended):

python -m venv env
source env/bin/activate  # Mac/Linux
.\env\Scripts\activate   # Windows
Install the required dependencies:

pip install -r requirements.txt
Project Structure 🗂️
Course-Recommendation-System/
├── Data/
│   └── Coursera.csv                                  # Coursera dataset
├── models/
│   ├── course_list.pkl                               # Precomputed similarity matrix
│   └── courses.pkl                                   # Processed course list
├── main.py                                           # Streamlit app script
├── CourseRecommendationSystem.py                     # Data preprocessing and model training script 
├── requirements.txt                                  # Python dependencies
├── Dockerfile                                        # Docker configuration
└── README.md                                         # Project README file
Usage ⚙️
Run the preprocessing and model training script:

python CourseRecommendationSystem.py
Run the Streamlit application:

streamlit run main.py
Navigate to the local URL (http://localhost:8501) to use the web app.

Docker Hub 🐳
To directly use the project from Docker Hub

Pull the pre-built Docker image:

docker pull ganeshpinnamaneni/course-recommendation-system:latest
Run the Docker container:

docker run -p 8501:8501 ganeshpinnamaneni/course-recommendation-system:latest
Access the web app at http://localhost:8501.

Contributing 🤝
We welcome contributions to improve the Course Recommendation System. Here's how you can contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Commit your changes (git commit -m 'Add new feature').
Push to the branch (git push origin feature-branch).
Create a Pull Request.
