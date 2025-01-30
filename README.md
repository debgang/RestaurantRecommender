# RestaurantRecommender
Chatbot which recommends the ideal restaurant for user based on user inputs and given restaurant data 

# Overview
Design a chatbot which will recommend Restaurants in Bangalore for given 
preferences for user. The chatbot will ask relevant questions from user to gather the user 
preferences and it will try to match it with existing dataset and provide top 3 
recommendations.

# Design

Check the design document

# Dataset

The dataset contains the Zomato Bangalore restaurants data from Kaggle Dataset below 
for Zomato restaurants in Bangalore
https://www.kaggle.com/datasets/himanshupoddar/zomato-bangalore-restaurants.
The dataset is cleaned to remove all empty columns and data type modifications for few 
columns. The dataset is randomly sampled to get 100 random records which is used as 
master data. Final dataset is uploaded.

# Sample interaction

Chatbot sample  
**Bot** : Hello! I'm here to help you find the perfect restaurant in Bangalore. Could you please 
share your preferred location or any specific area you're interested in?  

**User** : I am interested in BTM area    

**Bot** : Great! We have many restaurants in the BTM area. Do you prefer online ordering and 
table booking?    
**User** : No    
**Bot** : Thank you for the information. What type of cuisine do you prefer (e.g., North Indian, 
South Indian, Continental, Chinese, etc.)?  
**User** : North India,Chinese  
**Bot** : Thank you for sharing your cuisine preferences. What type of restaurant do you prefer 
(e.g., Fine Dining, Casual Dining, Street food, Quick Bites, Dhaba)?  
**User** : Casual Dining  
**Bot** : Thank you for the information. Do you have any preference for the minimum rating for 
the restaurant? If yes, please provide a minimum rating in the range of 2 to 5.  
**User** : Minimum rating of 3  
**Bot** : Thank you for the information. What is your approximate budget for 2 people?  
**User** : 800  
**Bot** : Thank you for providing all the details. Here's the profile based on your preferences:  
{'Location': 'BTM', 'Online Order Accepted': 'No', 'Table booking allowed': 'No', 'Cuisine': 
'North Indian, Chinese', 'Restaurant type': 'Casual Dining', 'Rating': 'Medium', 'Average cost 
for 2': '800'}   
**Bot** : Thank you for providing all the information. Kindly wait, while I will share with you the 
recommended restaurants:   
Based on your preferences, here are the top 3 recommended restaurants in BTM:  
1. **Birinz**: Located at 1st Floor, BTM Complex, 9th Main Road, 1st Stage, BTM, 
Bangalore. Phone: +91 8197022223, +91 9141111222. This casual dining restaurant offers 
a variety of cuisines including Biryani, Chinese, Mughlai, Fast Food, and Kebab. It has a 
high rating and an average cost for two is ₹700.
2. **Capsicum Family Restaurant**: Situated at 774, 3rd Floor, 16th Main, 7th Cross, 2nd 
Stage, BTM, Bangalore. Phone: 080 49652486. This casual dining spot serves Biryani and 
North Indian cuisine. It has a medium rating and the average cost for two is ₹800.
3. **Savoury Restaurant**: Located at 84, Hosur Main Road, Madivala, BTM, Bangalore. 
Phone: 080 49994999. This casual dining restaurant offers Arabian, North Indian, Chinese, 
and Fast Food cuisines. It also has a medium rating with an average cost for two at ₹800.
Please note that while these restaurants accept online orders, they do not allow table 
bookings.
**User** : exit  
**Bot** : If you have any more questions in the future, feel free to ask. Have a great day  

# Libraries used

- Python 3
- Langchain Azure Open AI

# Steps to run

- Get Azure Open AI subscription (https://azure.microsoft.com/en-us/pricing/details/cognitive-services/openai-service/)
- Set the following environment variables in your OS

   AZURE_API_VERSION  
   AZURE_DEPLOYMENT_NAME  
   AZURE_OPENAI_API_KEY  
   AZURE_OPENAI_ENDPOINT  

- Sync all files in the respository to a folder
- Run python file dialog_flow_restaurant.py
  python dialog_flow_restaurant.py

# Please reach out to below email address for any concerns
  debargha.ganguly@gmail.com
