Name|Matric Number
----|------
Nik Hamidi Wan Hamat| 1712475
Umar Hakimi Zahabuddin|  1714851
Syed Muhammad Arif Sayed Ali |1718247

## TITLE : IIUM Shutterstock
### Introduction
Throughout the years of study in IIUM, we realised that it will be great if IIUM community can stay connected and help each other with through the application. So, we agreed to develop an application called IIUM Shutterstock. This apps allow user to take photo and stored it on our database. The app required user to register for them to have access to the cloud storage. User can used their own account to view other's photo that have been uploaded to the application. Through this application, IIUM community can buy the photos from each other if they interested in using it for references or for other learning purpose. Users can upload the photos and its detail for other users to contact. We hoped that this application will familiarized IIUM community with the copyright issues and responsibility of using content from internet.

### Objective
This project are aim to help us to explore on the creation of mobile app using online database and also help user to store their image to the cloud either for privacy or storage issues. To create a community that show interest in photography and also to help IIUM community to share their good moments or good photos through this aplication. Next, IIUM community can stay connected to each other through this application. Lastly the most important part is want to familiarized IIUM community with the copyright issues and responsibility of using content from internet.
    
### Features and functionalities  
Features & Functionalities  | Explanation
 ---------------------------| -----------------------------------
 Register page              | User can register their own ID to log to our mobile application.
 Login page                 | Enable registered user to login into their own account.
 Anonymous login            | Enable the anonymous user to view the photos in the application
 React-Native-Camera        | to use the camera to capture the images
 Firebase                   | Use the authentication and database to store the images that user upload or capture through the application.
 Search page                | User can use our textinput to search any images that have been uploaded by other users.
 List page                  | Our mobile application will list and display all the uploaded photos in our application.
 View page                  | User can view the details of every photos from other users.
    
### Component and API
Component and API                                                          | Explanation
---------------------------------------------------------------------------|------------------------------------------------------------
import { NavigationContainer } from '@react-navigation/native';            |This component we used to track our screen. It can be used to moved to another specific screen that we need for our application
import { createStackNavigator } from '@react-navigation/stack';            |It was used for transition wihtin our application between the screens.          
import React, { Component } from 'react';                                  | Common used when we are using jsx
import {widthPercentageToDP as wp, heightPercentageToDP as hp} from 'react-native-responsive-screen';  | This component we used to specify the percentage of our width and height every view in our project. So the size of our view will be changed according to the mobile phone used         
import Icon from 'react-native-vector-icons/Ionicons';          | We used it for icon to be displayed
import LinearGradient from 'react-native-linear-gradient';      | We want to make a gradient color for our specific background screen
import { View, Text, StyleSheet,TextInput,TouchableOpacity, Btton, Alert, FlatList, ScrollView, StatusBar, Dimensions} from 'react-native';| All of those are important component where we want to dispay our content. Stylesheet used to create the style of our specific content. Textinput is needed for user to key in their id, password, to search items and to register the account. While TouchableOpacity is used to create a touchable space for the user to click on it, for example we created button using touchableOpacity to moved to another screen. Button obviouly we used to move to another screen or create an alert using it. While Flatlist is used to render many items that we want to display on our application. Next, ScrollView is used to enble the scroll feature for user to view more content on the screen. We set the Statusbar of our apps. We get the screen height using the Dimensions.                     
import auth from '@react-native-firebase/auth';             |Using this component, we can get authentication from our firebase for the user to log into their account.
import * as Animatable from 'react-native-animatable';      |used to create screen animation for our splashscreen,login page screen and profile page.
import { useTheme } from '@react-navigation/native';        |To access the currently active theme     
import MaterialIcons from 'react-native-vector-icons/MaterialIcons';    |  This component also we used their library to import the icon 
import { Card, Divider,IconButton} from 'react-native-paper';           |component card is a sheet of material that serves as an entry point to more detailed information.
import { FAB } from 'react-native-paper';                               |  To created a floating button of our application. The button used for the camera feature where user can capture the images and upload it on our application        
import { createMaterialBottomTabNavigator} from '@react-navigation/material-bottom-tabs';  | We create our main pages using the bottom navigation where user can select Home, Search and Profile pages at the bottom bar.

### Screen Navigation
![Screen Navigation](/2.jpg)
### Sequence Diagram
![Sequence Diagram](/5.jpg)
### References
1. https://www.codeproject.com/Articles/1267698/How-to-Build-a-React-Native-Image-Gallery-Tutorial
2. https://guides.github.com/features/mastering-markdown/
3. https://github.com/react-native-community/react-native-image-picker
4. https://firebase.google.com/docs/auth/web/start
5. https://reactnavigation.org/
6. https://reactnative.dev/
7. https://github.com/oblador/react-native-animatable
