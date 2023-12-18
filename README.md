-**University Name: [San Jose State University](http://www.sjsu.edu/)**  
-**Course: [Virtualization Technologies](http://info.sjsu.edu/web-dbgen/catalog/courses/CMPE283.html)**  
-**Professor [Mike Larkin]**  
-Students:
1. **[Anandu Sreekumar](https://github.com/AnanduSreekumar)**
2. **[Jeswanth Vadlamudi](https://github.com/jeswanthv)**

### Demo Screenshots:    
  
1. Homepage  
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/Homepage.png" alt="Homepage" height="405" width="720" />

2. New User Registration   
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/sign_up.png" alt="Signup_page_ss" height="405" width="720" />

3. Sign In
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/sign_in.png" alt="Login_page_ss" height="405" width="720" />

4. Identity Document Upload
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/doc_info_step%201.png" alt="ID_ipload page" height="405" width="720" />

5. Edit ID Card Details
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/edit_info%20step%202.png" alt="Edit_details" height="405" width="720" />

6. Destination Country/ Notary
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/info_step%203.png" alt="Edit_details" height="405" width="720" />

7. Payment
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/payment.png" alt="Edit_details" height="405" width="720" />

8. Notary Verification Page 1
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/notary_01.png" alt="Edit_details" height="405" width="720" />

9. Notary Verification Page 2
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/notary_2.png" alt="Edit_details" height="405" width="720" />

10. One-D Card
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/UI/one_D_card.png" alt="Edit_details" height="405" width="720" />




  
### AWS Setup:    
1. Cognito: Used for user identity pooling and management.
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/cognito.png" alt="Cognito_ss" height="405" width="720" />  
    
2. R53: Used for traffic management
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/r53.png" alt="Cognito_ss" height="405" width="720" />  
    
3. S3: For user files and secure object management
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/s3.png" alt="Cognito_ss" height="405" width="720" />

Implemented S3 bucket Lifecycle policy for Cost Optimization
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/S3_lifecycle.png" height="405" width="720" />
    
5. Lambda: For calling functions resulting is extracted text from user uploaded ID card
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/lambda_main.png" alt="Cognito_ss" height="405" width="720" />  
    
6. Textract: The AWS tool which extracts labelled data from given images
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/lambda.png" alt="Cognito_ss" height="405" width="720" />  
    
7. RDS: For maintaining a central database
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/RDS.png" alt="Cognito_ss" height="405" width="720" />  
    
8. Cloudwatch: To monitor Lambda calls and view logs
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/cloudwatch.png" alt="Cognito_ss" height="405" width="720" />  
    
9. Cloudfront: To deliver the user experience through a CDN
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/AWS%20Services/cloudfront.png" alt="Cognito_ss" height="405" width="720" />



### Technologies used:  

1. React: Used for frontend experience <img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/react.svg" alt="react" height="30" width="40" />

2. Flask: Used for backend Framework <img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/flask.svg" alt="flask" height="30" width="40" />

3. MySQL: Used for central database

### CI/CD: 
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/CICD.jpeg" alt="Cognito_ss" height="405" width="720" />

### Effort Distribution:  
<img align="center" src="https://github.com/AnanduSreekumar/ONE-D/blob/main/Screenshots_final/effort_distribution.png" alt="Edit_details" height="405" width="720" />

###  How to set up and run project locally?  

This project combines a React frontend and a Flask backend. To run it locally, make sure you have Node.js and npm installed for the frontend, and Python with pip for the backend. 

To set up the React frontend:
1. Navigate to the frontend directory and run npm install to install dependencies.
2. Start the development server with run dev (available at http://localhost:3000).

For the Flask backend:
1. In the backend directory, create a virtual environment with python -m venv venv.
2. Activate the virtual environment (use .\venv\Scripts\activate on Windows, or source venv/bin/activate on macOS/Linux).
3. Install Python dependencies with pip install -r requirements.txt.
4. Run the Flask app with python app.py (available at http://localhost:5000).

Access the application by opening your web browser at http://localhost:3000. The React frontend communicates with the Flask backend. For additional details or troubleshooting, refer to the documentation or this repository's additional information section.




## License

[MIT](https://choosealicense.com/licenses/mit/)
