# Twimba 🐦

Twimba is a **Twitter-like social feed web application** built using **Vanilla JavaScript**, HTML, and CSS.  
Users can post tweets, like them, retweet them, and view replies dynamically without reloading the page.

This project demonstrates **DOM manipulation, event delegation, state management, and modular JavaScript**.

---

## Features

- Post new tweets
- Like and unlike tweets
- Retweet and undo retweets
- View and hide replies
- Real-time UI updates
- Unique tweet IDs using UUID
- Clean and interactive UI

---

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- Font Awesome (icons)
- UUID (for unique tweet IDs)
- JavaScript Modules

---

## Project Structure
twimba/
│
├── index.html
├── index.css
├── index.js
├── data.js
├── images/
│ └── scrimbalogo.png
└── README.md


---

## How It Works

### Event Delegation
A single `click` event listener handles:
- Likes
- Retweets
- Replies
- Tweet creation

This makes the app efficient and scalable.

### Tweet Data Management
All tweets are stored in a `tweetsData` array imported from `data.js`.

Each tweet object contains:
- `handle`
- `profilePic`
- `likes`
- `retweets`
- `tweetText`
- `replies`
- `isLiked`
- `isRetweeted`
- `uuid`

---

## Core Concepts Used

- DOM manipulation
- Conditional rendering
- Array methods (`filter`, `forEach`, `unshift`)
- Template literals
- UUID generation
- Toggle UI states
- Modular JavaScript

---

##  Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Damu987/Twimba.git


 * Open index.html in your browser.
 * Start tweeting, liking, and retweeting!
 *  Sample Code Snippet
function handleLikeClick(tweetId){
    const targetTweetObj = tweetsData.filter(tweet => tweet.uuid === tweetId)[0]

    if(targetTweetObj.isLiked){
        targetTweetObj.likes--
    } else {
        targetTweetObj.likes++
    }

    targetTweetObj.isLiked = !targetTweetObj.isLiked
    render()
}

 ## Screenshots

<img width="450" height="500" alt="Image8" src="https://github.com/user-attachments/assets/2c338b27-0c5c-4eef-b3ff-62e24362640c" />


## Future Enhancements
  * Add persistent storage (LocalStorage / Backend)
  * User authentication
  * Reply posting feature
  * Character limit for tweets
  * Dark mode

## Author

Damini S
Frontend Developer (Fresher)
Passionate about building interactive web applications

GitHub: https://github.com/Damu987


## License
This project is licensed under the MIT License.


 
