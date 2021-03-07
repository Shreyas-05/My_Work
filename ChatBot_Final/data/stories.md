## interactive_story_email
* greet
    - utter_greet
* restaurant_search{"cuisine": "italian", "location": "kochi"}
    - slot{"cuisine": "italian"}
    - slot{"location": "kochi"}
    - action_verify_location
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\nCafe 17 in Ground Floor, Unisquare Building, Opposite Sreedhareeyam Eye Hospital, Kathrikadavu, Kaloor, Kochi has been rated 4.5 and the average price for two people is: 700.\nBloomsbury's Global Kitchen & Bakehouse in S 74, Level 2, LuLu Mall, NH-17, Entrance Road, Edapally Junction, Edappally, Kochi has been rated 4.4 and the average price for two people is: 650.\nThe Grill Lab in Namaskar Building, S.N. Junction, Sonia Nagar, Palarivattom, Kochi has been rated 4.2 and the average price for two people is: 700.\nMocha Art Cafe in 6/127, Opposite Jew Synagogue, Mattancherry, Kochi has been rated 4.2 and the average price for two people is: 700.\nCafe Stories in HMT Road, Kalamassery, Kochi, Kochi has been rated 3.9 and the average price for two people is: 500.\nPizza Hut in Third Floor, LuLu Mall, NH-17, Edappally, Kochi has been rated 3.9 and the average price for two people is: 600.\nEURO TRIP by Kochi Brasserie in 5/7-F, North kalamassery, ernakulam, kochi has been rated 3.7 and the average price for two people is: 500.\nEdam Art Cafe in 55/484, Old 39/5284, Ground Floor, Western Part, 8th Cross Road, Panampilly Nagar, Kochi has been rated 3.6 and the average price for two people is: 500.\nNYA Cafe in 671/B Manovihar Building, Hilllpalace Road Tripunithura, Kochi has been rated 3.6 and the average price for two people is: 350.\nUpstairs Italian Pizzeria in 1/453 ,Bastian Street , Fortkochi, Kochi Circle, Ernakulam, Kochi has been rated 3.3 and the average price for two people is: 450.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "rourkela"}
    - slot{"location": "rourkela"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Chinese"}
    - slot{"cuisine": "Chinese"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\nSai Restaurant in Sector 4, Rourkela -7690002, Raurkela Industrialship, Rourkela has been rated 4.1 and the average price for two people is: 350.\nChina Town Restaurant in Sector 4, Raurkela Industrialship, Rourkela has been rated 4.1 and the average price for two people is: 400.\nTamarind Sky Restro in Civil Township Rourkela, Raurkela Industrialship, Rourkela has been rated 4.1 and the average price for two people is: 350.\nChhote Nawab in Above Allen Solly Udit Nagar Rourkela, Railway Colony, Rourkela has been rated 4.0 and the average price for two people is: 350.\nThe Cakery Bakery in Bisra Road, Beside L.G. Plaza, Raurkela Industrialship, Rourkela has been rated 4.0 and the average price for two people is: 300.\nDaawat in Anand Bhawan Lane, Main Road, Hotel Rainbow Regency, Rourkela, Odisha 769001, Raurkela Industrialship, Rourkela has been rated 4.0 and the average price for two people is: 300.\nGarden Restaurant And Bar in Dav Chowk, Jail Road, Raurkela Industrialship, Rourkela has been rated 4.0 and the average price for two people is: 350.\nMadhuban Restaurant in Ground Floor, Madhuban Chowk, 4, Rourkela - 769004, Near Cell Quarter, Raurkela Industrialship, Rourkela has been rated 3.9 and the average price for two people is: 600.\nHideaway Restaurant & Cafe in C-1, Civil Township, Rourkela - 769004, Near Shani Mandir, Raghunathpali, Rourkela has been rated 3.9 and the average price for two people is: 350.\nFlavour Box in Near Federal Bank Civil Township Rourkela, Raghunathpali, Rourkela has been rated 3.8 and the average price for two people is: 500.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_wrong_location
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "bamboo"}
    - slot{"location": "bamboo"}
    - action_verify_location
    - utter_ask_proper_location
* restaurant_search{"location": "asansol"}
    - slot{"location": "asansol"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nRoyal Hotel in Bastin Bazar, Asansol Locality, Asansol has been rated 4.7 and the average price for two people is: Rs.400.\nDomino's Pizza in Unit No. G07, Ground floor, Galaxy Mall, District - Burdwan, Near Chitra More, Burnpur Road, 713325, Asansol Locality, Asansol, 713325 has been rated 4.3 and the average price for two people is: Rs.400.\nPratims Pizza in Gitashree apartment, S. B. Gorai road, Hillview east., Asansol Locality, Asansol has been rated 4.1 and the average price for two people is: Rs.300.\nHimland in SB Gorai Road, Sreepally, Asansol, Asansol Locality, Asansol has been rated 4.1 and the average price for two people is: Rs.300.\nNew Sudhamrit Restaurants in 30, Bastin Bazar, G T Road, Asansol - 713301, Asansol Locality, Asansol has been rated 4.1 and the average price for two people is: Rs.350.\nDelhi Hotel in 1, G.C. mitra road(hutton road), asansol, Asansol Locality, Asansol has been rated 4.0 and the average price for two people is: Rs.300.\nChicken Hub in Opp City Bus Stand, G T Road, beside electric office, Asansol Locality, Asansol has been rated 4.0 and the average price for two people is: Rs.300.\nMidos The Family Restaurant in Mahisila Colony, Munshi Bazar, Asansol Chittaranjan Road, Asansol Bazar, Asansol - 713301, Asansol Locality, Asansol has been rated 4.0 and the average price for two people is: Rs.700.\nLegends of Bengal in 15, Burnpur Road, opp Police lines, Asansol Locality, Asansol has been rated 4.0 and the average price for two people is: Rs.300.\nTheque in BNR More, Gt Road, Asansol - 713301, Opposite Rabindra Bhavan, Asansol Locality, Asansol has been rated 3.9 and the average price for two people is: Rs.400.\n"}
    - action_sendemail
    - utter_email_sent
* goodbye
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "ajmer"}
    - slot{"location": "ajmer"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nMango Masala Restaurant in 429/A/11 Vinod Bhawan, Kutchery Road has been rated 4.5 and the average price for two people is: Rs.600.\nSunny Di Hatti Amritsari in Near ICICI Bank, Kashyap Compound, Vaishali Nagar, Ana Sagar Lake, Ajmer has been rated 4.3 and the average price for two people is: Rs.400.\nMamta Sweets in Janta Colony, Vaishali Nagar, Ana Sagar Lake, Ajmer has been rated 4.3 and the average price for two people is: Rs.400.\nDomino's Pizza in Vega Mall, Near Suchna Kendra, Sardar Patel Marg, Ana Sagar Lake, Ajmer has been rated 4.2 and the average price for two people is: Rs.400.\nBurger King in Showroom 1A, Ground Floor, City Square Mall, A-Block, Panchsheel Nagar, Ajmer has been rated 4.2 and the average price for two people is: Rs.350.\nCafe Ate Pm in Alwar Gate, Opposite to Saint Paul School, Arya Nagar, Dhola Bhata Colony, Ajmer has been rated 4.2 and the average price for two people is: Rs.300.\nBaawarchi Brothers in St Stephens road, Ajmer has been rated 4.2 and the average price for two people is: Rs.350.\nGuddan Ka Dhaba in Opposite City Power House, Jaipur Road, Ana Sagar Lake, Ajmer has been rated 4.1 and the average price for two people is: Rs.300.\n7 Spices in Siddhi Complex, Near Ajanta Cinema, Dhola Bhata Colony, Ajmer has been rated 4.1 and the average price for two people is: Rs.500.\nRoll Express in Ground Floor, C 16, Vaishali Nagar, Ana Sagar Lake, Ajmer has been rated 4.1 and the average price for two people is: Rs.300.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_no_email
* greet
    - utter_greet
* restaurant_search{"location": "Amravati"}
    - slot{"location": "Amravati"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye

## interactive_story_no_email_2
* greet
    - utter_greet
* restaurant_search{"location": "ludhiana"}
    - slot{"location": "ludhiana"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "High"}
    - slot{"price_range": "High"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye

## interactive_story_no_email_3
* greet
    - utter_greet
* restaurant_search{"cuisine": " North Indian", "location": "faridabad"}
    - slot{"cuisine": " North Indian"}
    - slot{"location": "faridabad"}
    - action_verify_location
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye
* goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"cuisine": "chinese", "location": "Bokaro Steel City"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "Bokaro Steel City"}
    - action_verify_location
    - utter_ask_price_range
* restaurant_search{"price_range": "High"}
    - slot{"price_range": "High"}
    - action_search_restaurants
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nRainbow Restaurant in B 23, City Centre, Sector 4, Opp Bank Of Baroda, Bokaro Locality, Bokaro has been rated 4.1 and the average price for two people is: Rs.500.\nNirola in Plot No E/8, City Centre, Sector 4, Near United Bank Of India, Sector 8, Bokaro Locality, Bokaro has been rated 4.0 and the average price for two people is: Rs.400.\nA K Food Court in Sultan nagar, Chas, Bokaro, Bokaro Locality, Bokaro has been rated 4.0 and the average price for two people is: Rs.300.\nFoodie Junction in City Centre, Sector 4, Bermo has been rated 3.7 and the average price for two people is: Rs.300.\nShahi Darbar in Ground Floor, Gb 3, Sector 4, Bokaro - 827004, Near Police Club, Bokaro Locality, Bokaro has been rated 3.6 and the average price for two people is: Rs.450.\nSatkar Restaurant in Near Garga Over Bridge, Chas, Bokaro Locality, Bokaro has been rated 3.5 and the average price for two people is: Rs.300.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Bhubaneswar"}
    - slot{"location": "Bhubaneswar"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nRaghav's - Hotel Priya in Plot A-30/1, Unit 03, Unit 4, Bhubaneshwar has been rated 4.4 and the average price for two people is: Rs.500.\nNarula's Restaurant in Hotel Basera, 45-46, Ashok Nagar, Bhubaneshwar has been rated 4.4 and the average price for two people is: Rs.600.\nBOCCA Cafe in 108/B, 1st Floor, Janpath Road, Master Canteen Area, Kharabela Nagar, Bhubaneshwar has been rated 4.4 and the average price for two people is: Rs.450.\nSilver Streak in Ground Floor, BMC Bhawani Mall, Sahid Nagar, Bhubaneshwar has been rated 4.3 and the average price for two people is: Rs.500.\nDomino's Pizza in Plot M/18, PGL City Mart, NH 5, Oppostie Baramunda Fire Station, Baramunda, Bhubaneshwar has been rated 4.3 and the average price for two people is: Rs.400.\nAdda Unplugged in 3rd Floor,MRLA Complex,Patia,Bhubaneswar,751024 has been rated 4.2 and the average price for two people is: Rs.500.\nUpre Kitchen & Cafe in 3rd Floor, G-51, Near IOCL Office, Chandrasekharpur, Bhubaneshwar has been rated 4.2 and the average price for two people is: Rs.600.\nAdda Unplugged in Above Reliance Fresh, Near ITER College, Jagmohan Nagar, Bhubaneshwar has been rated 4.2 and the average price for two people is: Rs.500.\nKFC in Pal Heights, J/7, Jayadev Vihar, Bhubaneshwar has been rated 4.1 and the average price for two people is: Rs.450.\nCountry Kitchen in Khandagiri Marg, Jagmohan Nagar, Bhubaneshwar Bhubaneswar has been rated 4.1 and the average price for two people is: Rs.350.\n"}
    - action_sendemail
    - utter_email_sent
* goodbye
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Mangalore"}
    - slot{"location": "Mangalore"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Vadodara"}
    - slot{"location": "Vadodara"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\n22nd Parallel in 1st Floor, Tapan Complex, Besides M Cube Mall, Alkapuri, Vadodara has been rated 4.6 and the average price for two people is: Rs.400.\nJassi De Parathe in R.C Dutt Road, Near Kalaniketan, Alkapuri, Vadodara has been rated 4.5 and the average price for two people is: Rs.600.\nBrown Burger Co in Near Dairy Den Circle, Sayajiganj, Vadodara has been rated 4.4 and the average price for two people is: Rs.500.\nShree Kathiyawadi Khadki in Navrang Cinema Road, Near Tower Four Ways, Raopura, Mandvi, Vadodara has been rated 4.3 and the average price for two people is: Rs.300.\nKFC in 19, Ground Floor, Vadodara Central Mall, Near Genda Circle, Wadi Road, Alkapuri, Vadodara has been rated 4.3 and the average price for two people is: Rs.450.\nHariyali Restaurant in Vrundavan Heights, Near Parivar Char Rasta, Waghodia, Kendranagar, Vadodara has been rated 4.3 and the average price for two people is: Rs.400.\nDomino's Pizza in B-33, Ground Floor & 1st Floor, Uma Colony, Housing Society Limited, Waghodia Road, Kendranagar, Vadodara has been rated 4.3 and the average price for two people is: Rs.400.\nBurger King in 2nd Floor, Inorbit Mall, Subhanpura, Vadodara has been rated 4.2 and the average price for two people is: Rs.350.\nUstaad Miyaan in 13 Alkapuri shopping center, opposite vishwas colony, Alkapuri, vadodara, Alkapuri, Vadodara has been rated 4.2 and the average price for two people is: Rs.600.\nBurger King in Shop 8, Ground Floor, Golden Icon, Opposite BSNL Office, Bird Circle, Alkapuri, Vadodara has been rated 4.2 and the average price for two people is: Rs.350.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Bareilly"}
    - slot{"location": "Bareilly"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": " North Indian"}
    - slot{"cuisine": " North Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"price_range": " Medium", "cuisine": "south indian", "location": "Bangalore"}
    - slot{"cuisine": "south indian"}
    - slot{"location": "Bangalore"}
    - slot{"price_range": " Medium"}
    - action_verify_location
    - action_search_restaurants
    - utter_ask_price_range
* restaurant_search{"price_range": "High"}
    - slot{"price_range": "High"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "moradabad"}
    - slot{"location": "moradabad"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Chinese"}
    - slot{"cuisine": "Chinese"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye
    - action_restart

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"price_range": " Medium", "location": "nosik"}
    - slot{"location": "nosik"}
    - slot{"price_range": " Medium"}
    - action_verify_location
    - utter_ask_proper_location
* restaurant_search{"location": "ghaziabad"}
    - slot{"location": "ghaziabad"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - action_search_restaurants
    - utter_ask_price_range
* restaurant_search{"price_range": "High"}
    - slot{"price_range": "High"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nIndian Accent in The Lodhi, Lodhi Road, New Delhi has been rated 4.9 and the average price for two people is: Rs.5000.\nSevilla - The Claridges in The Claridges, 12, Dr. A.P.J. Abdul Kalam Road, Aurangzeb Road, New Delhi has been rated 4.7 and the average price for two people is: Rs.4500.\nDiggin in 10, Santushti Shopping Complex, Race Course Road, Chanakyapuri, New Delhi has been rated 4.5 and the average price for two people is: Rs.1300.\nCafe Wink in G-1, Plot 9, Sikka Galaxy, Shreshtha Vihar, Anand Vihar, New Delhi has been rated 4.5 and the average price for two people is: Rs.800.\nDiggin in Shop 1 & 2, Sri Fort Road, Opposite Gargi College, Anand Lok, New Delhi has been rated 4.4 and the average price for two people is: Rs.1400.\nGulati in 6, Pandara Road Market, New Delhi has been rated 4.4 and the average price for two people is: Rs.2500.\nSoho Bistro & Cafe in Khasra 264, Ground Floor, Westend Marg, Saidulajab, Saket, New Delhi has been rated 4.4 and the average price for two people is: Rs.1400.\nTamasha in 28, Block A, Kasturba Gandhi Marg, Connaught Place, New Delhi has been rated 4.4 and the average price for two people is: Rs.1600.\nThe G.T. Road in M 39, Outer Circle, Connaught Place, New Delhi has been rated 4.4 and the average price for two people is: Rs.1200.\nArdor 2.1 in N-55/56 & 88/89, Outer Circle, Connaught Place, New Delhi has been rated 4.3 and the average price for two people is: Rs.1800.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Bareilly"}
    - slot{"location": "Bareilly"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nDhaba Santa Banta Da in Krishna Vanti Colony, Model Town, Bareilly has been rated 4.3 and the average price for two people is: Rs.500.\nDelight Pizza Point in Karamchari nagar road, opp. Bhasin Traders, Hartman chauraha, Bareilly, Izatnagar, Bareilly has been rated 4.2 and the average price for two people is: Rs.350.\nMfc ( Mister Fried Chicken) in 2/105. Civil line, Near Ayu Khan Chauraha, Civil Lines, Bareilly - 243001, opp union bank of India, Subhash Nagar Colony, Bareilly has been rated 4.2 and the average price for two people is: Rs.450.\nKhana  Khazana in Phuta Darwaza, bazaar Sahukara, Jamuna Das Marg, Civil Lines, Bareilly has been rated 4.1 and the average price for two people is: Rs.500.\nVestal Fast Food in 614, Janakpuri, near selection point tower, Bareilly 243001, Subhash Nagar Colony, Bareilly has been rated 4.0 and the average price for two people is: Rs.500.\nAl Hamd Chicken Biryani Corner in Shop no 3, Near HDFC bank, near Ram janki mandir, Model Town, Bareilly has been rated 4.0 and the average price for two people is: Rs.350.\nBajrang Dhaba - Family Dhaba Restaurant in On Road, Pilibhit Bypass Road, Pilibhit Bypass, Bareilly - 243122, Near At Sanjay Nagar Tiraha Mod, Subhash Nagar Colony, Bareilly has been rated 3.8 and the average price for two people is: Rs.400.\nGanpati Sweets Restaurant in Opposite Roadways, Near imperial cinema, Civil Lines, Bareilly - 243001, Subhash Nagar Colony, Bareilly has been rated 3.8 and the average price for two people is: Rs.400.\nFlashback in 165-1 , Janakpuri , A2 building , Bareilly has been rated 3.8 and the average price for two people is: Rs.300.\nAtithi Express in Piliphit Road, Koharapeer, Bareilly - 243003, Near Munglum Sweets, Subhash Nagar Colony, Bareilly has been rated 3.7 and the average price for two people is: Rs.300.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"price_range": " Low", "location": "Belgaum"}
    - slot{"location": "Belgaum"}
    - slot{"price_range": " Low"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Chinese"}
    - slot{"cuisine": "Chinese"}
    - action_search_restaurants
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye
    - action_restart

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "Jalandhar"}
    - slot{"location": "Jalandhar"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Italian"}
    - slot{"cuisine": "Italian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nLovely Bake Studio in Nakodar Road, Jalandhar has been rated 4.6 and the average price for two people is: Rs.300.\nFood Bazar in Madan Flour Mill Compound, Ladowali Road, Central Town, Shastri Nagar, Jalandhar has been rated 4.5 and the average price for two people is: Rs.300.\nTummys Drive in Shop No-3, Ground Floor, 7 Gyan Nagar,  Jalandhar has been rated 4.5 and the average price for two people is: Rs.400.\nAar Kay Vaishno Dhaba in Near Nari Niketan, Nakodar Road, Jalandhar has been rated 4.4 and the average price for two people is: Rs.300.\nKFC in Rampa Centre Point, Model Town Market, Model Town, Jalandhar has been rated 4.4 and the average price for two people is: Rs.450.\nDomino's Pizza in 187 L, Ground Floor & 1st Floor, Model Town Market, Model Town, Jalandhar has been rated 4.4 and the average price for two people is: Rs.400.\nAggarwal Vaishno Dhaba in Vasant Vihar Road, Model Town, Jalandhar has been rated 4.3 and the average price for two people is: Rs.400.\nBurger King in Model Town Market, Model Town, Jalandhar has been rated 4.3 and the average price for two people is: Rs.350.\nBaithak in 8-9, New Colony, Near Johal Market,Jalandhar has been rated 4.3 and the average price for two people is: Rs.500.\nAmritsari Lovely Dhaba in Basti Adda Road, Near Football Chowk, Shakti Nagar, Shastri Nagar, Jalandhar has been rated 4.3 and the average price for two people is: Rs.700.\n"}
    - action_sendemail
    - utter_email_sent
* goodbye
    - utter_goodbye
    - action_restart

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"cuisine": "Kochi"}
    - slot{"cuisine": "Kochi"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}

## interactive_story_2
* greet
    - utter_greet
* restaurant_search{"price_range": " Medium", "cuisine": "North Indian", "location": "Kochi"}
    - slot{"cuisine": "North Indian"}
    - slot{"location": "Kochi"}
    - slot{"price_range": " Medium"}
    - action_verify_location
    - action_search_restaurants
    - utter_ask_price_range
* restaurant_search{"price_range": "High"}
    - slot{"price_range": "High"}
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye
    - action_restart

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"price_range": " Medium", "location": "Kozhikode"}
    - slot{"location": "Kozhikode"}
    - slot{"price_range": " Medium"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Italian"}
    - slot{"cuisine": "Italian"}
    - action_search_restaurants
    - utter_ask_price_range
* restaurant_search{"price_range": "High"}
    - slot{"price_range": "High"}
    - action_search_restaurants
    - utter_conf_email
* deny{"deny": "no"}
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"cuisine": "Italian", "location": "chennai"}
    - slot{"cuisine": "Italian"}
    - slot{"location": "chennai"}
    - action_verify_location
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nMezze in Old 19, New 4, Abhinav Center, Off Chamiers Road, Alwarpet, Chennai has been rated 4.5 and the average price for two people is: Rs.700.\nYaa Mohaideen Biryani in Old Shop 4/158, Church Road, Opposite Uzhavar Santhai, Pallavaram, Chennai has been rated 4.4 and the average price for two people is: Rs.600.\nWriter's Cafe in 98, Peter's Road, Near Philip's Service Centre, Gopalapuram, Chennai has been rated 4.4 and the average price for two people is: Rs.600.\nFusilli Reasons in 2/64, Ormes Main Road, Kilpauk, Chennai has been rated 4.4 and the average price for two people is: Rs.400.\n"}
    - action_sendemail
    - utter_email_sent
* affirm{"affirm": "thanks"}
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "kakinada"}
    - slot{"location": "kakinada"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nYati Foods - Bhanugudi in Bharati Axis Limited Opposite, Beside Aishwarya Grand and Petrol Bunk, Bhanu Gudi Junction has been rated 4.3 and the average price for two people is: Rs.400.\nKFC in 82, SRMT Mall & Multiplex, Near, Sarpavaram Junction, Ramanayyapeta, Kakinada Locality, Kakinada has been rated 4.3 and the average price for two people is: Rs.450.\nDomino's Pizza in Door 2, Upper Ground Floor, Sri Rangarayanim Residency, 1-47, Bhanugudi Junction, Srinagar, Kakinada Locality, Kakinada has been rated 4.3 and the average price for two people is: Rs.400.\nMcDonald's in Lalitha Nagar, Ramanayyapeta, Kakinada Locality, Kakinada has been rated 4.3 and the average price for two people is: Rs.500.\nKshatriya Foods in Door No : 67 11 7/c, 5th Cross Road, Venkat Nagar, Kakinada - 533003, Opposite Jntu 2nd Gate, Kakinada Locality, Kakinada has been rated 4.2 and the average price for two people is: Rs.400.\nBarkaas Arabic Restaurant in 28-1-10, Main Rd, Suryanarayana Puram, Kakinada Locality, Kakinada has been rated 4.1 and the average price for two people is: Rs.500.\nEat More in Opposite KKR Gowtham School, Near Pragathi Inter College, D- Mart Road, Venkat Nagar, Kakinada Locality, Kakinada has been rated 4.1 and the average price for two people is: Rs.300.\nFood Park Family Restaurant in Shop No:1, Ontimamedi Junction, Pratap Nagar, Kakinada - 533004, Near Gandhi Nagar Park, Kakinada Locality, Kakinada has been rated 4.0 and the average price for two people is: Rs.350.\nReeves in Suryarao Peta, Lachiraju Vari Street, Opposite Reliance Shopping Center, Kakinada Locality, Kakinada has been rated 4.0 and the average price for two people is: Rs.500.\nMeesala Raju Gari Hotel Ashoka Inn in Shankar Plaza, Ground Floor, Opposite Subhadrarcade, Pithapuram Road, Bhanugudi Junction, Kakinada Locality, Kakinada has been rated 3.9 and the average price for two people is: Rs.600.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "rajkot"}
    - slot{"location": "rajkot"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Chinese"}
    - slot{"cuisine": "Chinese"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nTGT - The Grand Thakar in Opposite Jubilee Garden, Jawahar Road, Sadar, Kothi Compound, Rajkot has been rated 4.6 and the average price for two people is: Rs.700.\nSargam Food in Shop 9, Ground Floor, Bilkha Plaza, Kasturba Road, Junction Plot, Rajkot has been rated 4.5 and the average price for two people is: Rs.300.\nJassi De Parathe in Mangal Bhavan Apartment, Nirmala School Road, Kotecha Nagar, Rajkot has been rated 4.5 and the average price for two people is: Rs.600.\nLa Pino'z Pizza in Chandra Park-2 Corner, Near Big Bazaar, Opposite Reliance Mall, 150 Feet Ring Road, Rajkot has been rated 4.4 and the average price for two people is: Rs.500.\nDNS- Desserts N Shakes in Shop 5, Near Jagnath Police Chowki, Dr Yagnik Road, Rajkot has been rated 4.4 and the average price for two people is: Rs.400.\nRajmandir Food Zone in Near Hemugadhvi Hall, Tagore Road, Astron Chowk, Rajkot has been rated 4.4 and the average price for two people is: Rs.500.\nMcDonald's in Ground & 1st Floor, Jupiter Atrium Everest Park, Nanamawa, Jakatnaka, Kalawad Road, Kotecha Nagar, Rajkot has been rated 4.3 and the average price for two people is: Rs.500.\nCheelizza in Nandan Nalinkant, Jalaram Plot-2 Corner, Near Shree Gita Oil Depot, University Road, Kotecha Nagar, Rajkot has been rated 4.3 and the average price for two people is: Rs.500.\nDomino's Pizza in Shop 1, Plot 23, 24, Ground Floor, Radhika House, Kalawad Road has been rated 4.3 and the average price for two people is: Rs.400.\nBig Bite in Race Course Ring Road, Near Indian Oil Petrol Pump, Sadar, Race Course, Rajkot has been rated 4.3 and the average price for two people is: Rs.500.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"cuisine": "Mexican", "location": "ahmedabad", "price_range": "Medium"}
    - slot{"cuisine": "Mexican"}
    - slot{"location": "ahmedabad"}
    - slot{"price_range": "Medium"}
    - action_verify_location
    - action_search_restaurants
    - utter_conf_email
* deny{"deny": "not needed"}
    - utter_goodbye

## interactive_story_1
* greet{"greet": "hai"}
    - utter_greet
* restaurant_search{"price_range": "Medium", "cuisine": "North Indian", "location": "Kolkata"}
    - slot{"cuisine": "North Indian"}
    - slot{"location": "Kolkata"}
    - slot{"price_range": "Medium"}
    - action_verify_location
    - action_search_restaurants
    - utter_conf_email
* deny
    - utter_goodbye

## interactive_story_1
* greet{"greet": "hai"}
    - utter_greet
* restaurant_search{"price_range": "High", "cuisine": "Italian", "location": "Kozhikode"}
    - slot{"cuisine": "Italian"}
    - slot{"location": "Kozhikode"}
    - slot{"price_range": "High"}
    - action_verify_location
    - action_search_restaurants
    - utter_conf_email
* deny{"deny": "no"}
    - utter_goodbye


## interactive_story_1
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "bilaspur"}
    - slot{"location": "bilaspur"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Chinese"}
    - slot{"cuisine": "Chinese"}
    - utter_ask_price_range
* restaurant_search{"price_range": "Medium"}
    - slot{"price_range": "Medium"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nGIZA in Near Taj Masjid , Talapara , Bilaspur has been rated 4.5 and the average price for two people is: Rs.400.\nKrishna Veg Restaurant in Old Bus Stand, Telipara, Bilaspur has been rated 4.3 and the average price for two people is: Rs.350.\nMaosaji (SVM) in Shrikant Verma Marg, Bilaspur H O, bilaspur-chhattisgarh - 495001, Near Rama Magneto Mall, Telipara, Bilaspur has been rated 4.2 and the average price for two people is: Rs.500.\nKFC in Ground Rama Magneto Mall, Srikant Verma Marg, Talapara, Tifra, Bilaspur has been rated 4.2 and the average price for two people is: Rs.450.\nRasoi Veg Restaurant in Indra Gandhi Chowk , Tarbahar , Bilaspur , Chhattisgarh , 495001 has been rated 4.2 and the average price for two people is: Rs.500.\nMadrasi Treat in Agrasen Chowk , Bilaspur has been rated 4.1 and the average price for two people is: Rs.350.\nRoll Sholl in Sai Palisar, Shrikant Verma Marg, Vaishali Nagar, Bilaspur-Chhattisgarh - 495004, Beside Oriental Bank Of Commerce, Agyay Nagar, Bilaspur has been rated 4.1 and the average price for two people is: Rs.300.\nThe Momo's Panda & The Curry House in Link Road, CMD Chowk, Bilaspur- 495001, Telipara, Bilaspur has been rated 4.0 and the average price for two people is: Rs.300.\nBox Office in Opposite Shri Krishna Netralaya, Link Road, Bilaspur, Chhattisgarh has been rated 4.0 and the average price for two people is: Rs.300.\nMaosaji in Maosaji Mangla Chowk, mungeli road, bilaspur chhattisgarh, Narmada Nagar, Bilaspur has been rated 4.0 and the average price for two people is: Rs.400.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "bellanduru"}
    - slot{"location": "bellanduru"}
    - action_verify_location
    - utter_ask_proper_location
* restaurant_search{"location": "Mumbai"}
    - slot{"location": "Mumbai"}
    - action_verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "North Indian"}
    - slot{"cuisine": "North Indian"}
    - utter_ask_price_range
* restaurant_search{"price_range": "High"}
    - slot{"price_range": "High"}
    - action_search_restaurants
    - utter_conf_email
* affirm
    - utter_ask_id
* restaurant_search{"email": "foody.chatbot@gmail.com"}
    - slot{"email": "foody.chatbot@gmail.com"}
    - action_fill_email_body
    - slot{"emailbody": "Showing you top rated restaurants:\n\nMirchi And Mime in G6,One Boulevard,Lake Boulevard Road, Hiranandani Business Park, Powai, Mumbai has been rated 4.9 and the average price for two people is: Rs.1800.\nBastian in B/1, New Kamal Building, Opposite National College, Linking Road, Bandra West, Mumbai has been rated 4.8 and the average price for two people is: Rs.4200.\nAer - Four Seasons in 1/136, E Moses Road, Worli, Mumbai has been rated 4.7 and the average price for two people is: Rs.4500.\nHakkasan in 206, 2nd Floor, Krystal, Waterfield Road, Linking Road, Bandra West, Mumbai has been rated 4.7 and the average price for two people is: Rs.2600.\nGallops in Mahalaxmi Race Course, Mahalaxmi, Mumbai has been rated 4.6 and the average price for two people is: Rs.2600.\nThe Fusion Kitchen in Shop 1, Opposite Veda Building, Near Bhavdevi Garage, Holy Cross Road, IC Colony, Borivali West, Mumbai has been rated 4.6 and the average price for two people is: Rs.1600.\nSammy Sosa in Shop 18, Meera CHS, Near Mega Mall, Oshiwara Link Road, Oshiwara, Andheri West has been rated 4.6 and the average price for two people is: Rs.1600.\nJoey's Pizza in Shop 1, Plot D, Samruddhi Complex, Chincholi Bunder Road, Mindspace, Malad West, Mumbai has been rated 4.4 and the average price for two people is: Rs.800.\nVeranda in 331, Dr Ambedkar Road, Pali Hill, Bandra West, Mumbai has been rated 4.4 and the average price for two people is: Rs.2200.\nYauatcha in 206, 2nd Floor, Krystal, Waterfield Road, Linking Road, Bandra West, Mumbai has been rated 4.4 and the average price for two people is: Rs.2800.\n"}
    - action_sendemail
    - utter_email_sent
* affirm
    - utter_goodbye
