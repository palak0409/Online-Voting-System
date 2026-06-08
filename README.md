# To see the website -> https://online-voting-w306.onrender.com

# Online-Voting
The Online Voting System is a secure and user-friendly web application that enables digital elections. It allows administrators to create and manage elections, add candidates, and monitor live results, while voters can securely cast their votes online.

This project is designed as a group project to demonstrate concepts of web development, database management, and data visualization.

**👥 Group Members**                                                                                                                                         
**1. Palak Tiwari**                                                                                                                                            
2. Sonu  Kumar                                                                                                                                          
**3. Sonali Sharma**                                                                                                                                          


**🧰 Technologies Used**

|**Category**	       |         **Technologies**                    |                                                                                          
|--------------------|---------------------------------------------|
|Frontend	           |  HTML5, CSS3, Bootstrap                     |                                                                                          
|Backend	           |  Python (Flask Framework)                   |                                                                                          
|Database	           |  SQLite3                                    |                                                                                          
|Visualization  	   |  Chart.js (Pie and Line Charts)             |                                                                                          
|Security	           |  Session management, CAPTCHA authentication |                                                                                          
|Version Control	   |  Git & GitHub                               |  

**⚙️ Features**

**👨‍💻 User Side**

. User Registration & Login (with CAPTCHA verification)                                                                                                       
. Secure session-based authentication                                                                                                                         
. Dynamic election selection                                                                                                                                  
. Real-time voting system (one vote per election)

**🧑‍💼 Admin Side**

. Admin login with session control                                                                                                                            
. Create and manage elections                                                                                                                                 
. Add and remove candidates                                                                                                                                   
. Monitor live vote counts                                                                                                                                    
. View election statistics and winner results                                            

**🗂️ Database Schema**

**Tables:**

**1. users**

  . id – Primary Key                                                                                                                                           
  . username – Unique Username                                                                                                                                 
  . password – Encrypted Password

**2. elections**

  . id – Primary Key                                                                                                                                           
  . name – Election Name                                                                                                                                       
  . start_time – Election Start Date/Time                                                                                                                      
  . end_time – Election End Date/Time                                                                                                                          

**3. candidates**

  . id – Primary Key                                                                                                                                           
  . name – Candidate Name                                                                                                                                      
  . election – Linked Election Name                                                                                                                            
  . votes – Vote Count                                                                                                                                         

**🚀 Working Procedure**

**1️⃣ Setup**

  1. Install Python (3.8 or above)                                                                                                                             
  2 . Clone this repository
  
    git clone https://github.com/Amritanshu319/Online-Voting.git

  3. Navigate to the project folder
     
    cd Online-Voting

  4. Install dependencies

    pip install flask

**2️⃣ Run the Application**

    python app.py

  Then open your browser and visit:

    http://127.0.0.1:5000/
     
**3️⃣ User Flow**

1. Register a new user account
2. Login using your credentials and complete the CAPTCHA
3. Choose an election and cast your vote
4. Once submitted, votes are stored securely in the SQLite database
5. Users can view results as real-time

**4️⃣ Admin Flow**

1. Log in as an Admin
2. Create elections and add candidates
3. Monitor live voting results
4. View visual statistics (Pie & Line charts)
5. Declare winners based on live vote counts

**📊 Visualization**

The voting results are represented dynamically using Chart.js:
  . Pie Chart – Displays candidate vote share
  . Line Chart – Tracks votes trend for each election

**🧩 Folder Structure**

    Online-Voting/
    │
    ├── app.py                  # Main Flask application
    ├── templates/              # HTML templates
    │   ├── admin_dashboard.html
    │   ├── admin_login.html
    │   ├── base.html
    │   ├── create_election.html
    │   ├── election_chart.html
    │   ├── index.html
    │   ├── login.html
    │   ├── manage_candidates.html
    │   ├── manage_elections.html
    │   ├── manage_users.html
    │   ├── register.html
    │   ├── thank_you.html
    │   ├── user_dashboard.html
    │   ├── view_results.html
    │   ├── vote.html
    │   └── vote_success.html
    ├── static/                 # CSS, JS, images
    │   ├── admin_dashboard.css
    │   ├── admin_login.css
    │   ├── index.css
    │   ├── style.css
    │   ├── view_result.css
    │   └── voting.jpg
    ├── database.db             # SQLite database
    └── README.md               # Project documentation

**🔒 Security Features**

  . CAPTCHA validation during login                                                                                                                           
  . Session-based authentication                                                                                                                              
  . Restricted admin routes                                                                                                                                   
  . Prevention of multiple votes by a single user

**🧠 Future Enhancements**

  . Integration with Blockchain for immutable vote records                                                                                                    
  . Add email verification for user registration                                                                                                              
  . Implement role-based access control                                                                                                                       
  . Live election timers and countdowns
