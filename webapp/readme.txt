AUTHORS: Harry Tian & Daniel Kim

DATA: information about trending Youtube videos from 2017.11.14 to 2018.06.14

The license for this data is CC0: Public Domain.
The dataset can be downloaded here https://www.kaggle.com/datasnaek/youtube-new

STATUS: 
FEATURES CURRENTLY WORKING:
- At mainpage, renders trending videos from a default date.
- Maximum 10 videos are shown at once, and the prev/next buttons enable to switch to other videos in main page.
- Searching for trending videos on user-specified date & rendering the searched videos.
- Basic local sign up: creates an account for the user, stores it in the psql database, and returns a message.
- Basic local log in: checks the psql database if the username exists and returns a message.
- Log out 
- Vertical view: shows the list of trending videos vertically.
- Create playlist: creates a playlist that stores selected videos.
- Delete playlist: deletes a playlist along with the videos in it
- Save to my playlist: saves a selected video to user's playlist.
- Remove from playlist: removes a select video from a playlist
- sharing data from index.html to mypage.html using local storage
- My page: a page that shows users' playlist and videos.

FEATURES NOT WORKING:
    User signup and login feature using flask-login

NOTES:
    Instead of using flask-login, we implemented login feature using localStorage: we store username into localStorage
    and access to it whenever we have to verify the user or keep the user data from refreshing the page. We remove the
    data from the localStorage when the user clicks the Log out button.