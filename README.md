# Moodify
Moodify: It is a computer vision app that sees you and then relaxes you

## How Project Works 
So, when a user starts using moodify, the user will come up with a window of a login screen which basically allows user to login his/her spotify credentials, if not sign up using Google, Apple ID, etc. 
As soon as the login is accepted a pop up comes which ask user’s to allow to open up the camera. Allowing will start detection of face and then mood will be shown whether it is bad, angry, etc. taking up 7 basic moods to detect the face and then showing the mood of the person. When this web app done detecting the face and mood it will generate a very generous spotify playlist according to the mood. It will generate a list of 30 songs based on a particular mood with all and all good accuracy. 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Technologies 
We integrated both frontend and backend for our project. When talking about front-end part this web application relies on a face-api.js which is a Javascript API used for detecting face and face recognition in the browser built on tensorflow.js and p5.js which are processing libraries for browser. Once a person clicks on Submit to Spotify button, we defined 7 basic moods to match a person’s facial expressions and for this we can use Spotify API to generate a spotify list. 


We used flask as out backend server and spotipy library to create the playlist. We firstly take the user’s spotify username and follow the spotify user authentication flow to obtain authorization to spotify API. Used access token to make API requests, once access tokens is acquired, we waited for a fefch post request from front-end when user clicks on the spotify button. On submitting fetch pst request, we creates a user’s top artist spotify list getting all 30 tracks within a certain mood.

