# Admin-Dashboard
Centralized Data and Monitoring for Admin used by Administrator to see the data insights and sales of the organization and it is also used for taking real-time decisionas from real time data insights and also is useful for tracking , sales , inventory , ratings etc and also the dashboard is personalized and tailored according to admin's need and requirements.

Steps to Start the project -

#step-1 :
  In client folder create a '.env.local' file and insert 'REACT_APP_BASED_URL'
  for example ( REACT_APP_BASE_URL = 'http://localhost:5001' )

#step-2 :
  In server folder create a '.env' file for 'MONGO_URL' & 'PORT' 
  for example ( MONGO_URL = 'your mongo atlas url'  PORT = any-port-number )

  for MONGO_URL perform following steps :
    #Step 1: Go to monngodb website and log in with your credentials or sign in 
    #Step 2: Create a database with a shared option (which is free) 
    #Step 3: Choose the desired location (Choose carefully and select the free options only)
    #Step 4: Click on Create clusters 
    #Step 5: Create your user with 'username and password'
    #Step 6: Scroll down and click on 'My Environment' and then click on 'Add My Current IP Address' 
    #Step 7: Navigate to 'Network Access' and click on 'ADD IP ADDRESS'
        #Step 1: In the 'Access List Entry:' type '0.0.0.0/0' (this is for accessing your database from any IP Address) 
        #Step 2: In the 'Comment:' section add anything you want or 'includes your current IP address'

#step-3 :
  Navigate to server folder & open the 'index.js' file 
  uncomment the following lines (
     AffiliateStat.insertMany(dataAffiliateStat);
     OverallStat.insertMany(dataOverallStat);
     Product.insertMany(dataProduct);
     ProductStat.insertMany(dataProductStat);
     Transaction.insertMany(dataTransaction);
     User.insertMany(dataUser);
  )

#step-4 :
  Open the code in your IDE & open terminal
    #step-1: type 'cd client' and press Enter -> then type 'npm i' and press Enter -> let the command download the dependencies
    #step-2: open new Terminal -> type 'cd server' and press Enter -> then type 'npm i' and press Enter -> let the command download the dependencies

#step-5 :
  In the server terminal type 'npm start' to push the data set in your Mongodb Cluster 
#step-6 : 
  Check your MongoDB atlas for the confiormaltion that data is uploaded in your cluster
  If uploaded -> stop the terminal -> after that Navigate to server folder & open the 'index.js' file -> comment the following lines (
                                                                                                           AffiliateStat.insertMany(dataAffiliateStat);
                                                                                                           OverallStat.insertMany(dataOverallStat);
                                                                                                           Product.insertMany(dataProduct);
                                                                                                           ProductStat.insertMany(dataProductStat);
                                                                                                           Transaction.insertMany(dataTransaction);
                                                                                                           User.insertMany(dataUser);
                                                                                                        )

#step-7 :
  Now open New Terminal and Split the terminal 
  in 1st terminal type 'cd server' -> then 'npm start'
  in 2nd terminal type 'cd client' -> then 'npm start'

Project will run on your Default browser :) 
  
