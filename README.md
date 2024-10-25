# Reddish - A Reddit Clone - MERN

Discussion Field using MERN stack and Elastic Search.

## Features

- Elastic Search
- Authentication (login/register with username-password)
- CRUD posts & comments
- Add posts in the form of text, link or image
- Upvote/downvote posts & comments
- Dynamic URLs for users (u/Aman) & subreddits (r/reactjs)
- Sorting of posts on basis of algorithms like hot, top, controversial etc.
- Full database search feature
- Pagination of posts
- Error management to prevent app crashes
- Sort comments by oldest, newest, most upvoted etc.
- Avatar uploading for user profiles
- Toast notifications for actions: adding posts, deleting comments etc.
- Loading spinners for relevant fetching processes
- Dark mode toggle w/ local storage save
- Responsive UI for all screens

## Screenshots

#### Desktop/Tablet

![Desktop-home](https://github.com/amand33p/reddish-mern/blob/master/screenshots/desktop-home.png)
![Desktop-2](https://github.com/amand33p/reddish-mern/blob/master/screenshots/desktop-2.png)
![Desktop-3](https://github.com/amand33p/reddish-mern/blob/master/screenshots/desktop-3.png)

#### Mobile

![Mobile-home](https://github.com/amand33p/reddish-mern/blob/master/screenshots/mobile-home.png)
![Mobile-2](https://github.com/amand33p/reddish-mern/blob/master/screenshots/mobile-2.png)
![Mobile-3](https://github.com/amand33p/reddish-mern/blob/master/screenshots/mobile-3.png)
![Mobile-4](https://github.com/amand33p/reddish-mern/blob/master/screenshots/mobile-4.png)
![Mobile-5](https://github.com/amand33p/reddish-mern/blob/master/screenshots/mobile-5.png)

## Usage

Notes:

- For image API, make account at cloudinary.com & get API keys from account dashboard.
- For upload preset usage, if you want to organize images separately at cloudinary.com, you have to create it from account settings first. If you don't want to, just don't put anything or use .env key - `UPLOAD_PRESET`.

#### Env variable:

Create .env file in server directory and add the following:

```
MONGODB_URI = "Your Mongo URI"
PORT = 3005
SECRET = "Your JWT secret"
CLOUDINARY_NAME = "From your cloudinary dashboard"
CLOUDINARY_API_KEY = "From your cloudinary dashboard"
CLOUDINARY_API_SECRET = "From your cloudinary dashboard"
UPLOAD_PRESET = "Folder/preset name from your cloudinary account" (OPTIONAL)
```

#### Client:

Open client/src/backendUrl.js & change "backend" variable to `"http://localhost:3005"`

```
cd client
npm install
npm start
```

#### Server:

Note: Make sure that you have installed 'nodemon' as global package.

```
cd server
npm install
npm run dev
```
