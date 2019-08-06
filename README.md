# React mp3 Player

An Mp3 player to play any audio file based on ReactJS

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Adding-new-icons-to-the-library](#Adding-new-icons-to-the-library)
- [Contributing](#contributing)

## Installation

Install via NPM

```shell
npm install react-mp3-player
```

or use yarn

```shell
yarn add react-mp3-player
```

## Usage

Import the Playlist component

```Javascript
import Playlist from 'react-mp3-player';
```

The tracks format will be ann array of objects, each object containing a name, description, src mp3 and an optional image

```Javascript
const tracks = [{ img: 'https://icon-library.net/images/music-icon-transparent/music-icon-transparent-11.jpg', name:'MP3', desc: 'Description 1', src:'Audio.mp3'},
{ img: 'https://icon-library.net/images/music-icon-transparent/music-icon-transparent-11.jpg', name:'MP3 #2', desc: 'Description 2', src:'Audio2.mp3'}]
```

Additional properties can be added to the component such as a right or left offset to decrease the width of the player as well as being able to choose the breakpoint for switching to mobile view, these options are passed into the playlist component in an object as props.

```Javascript
const playlistOverideStylingOpts = {
  offset : {
    left : 300
  },
  breakpoint : {
    maxWidth : 768
    }
};
```

Add the Player component and pass it the relative mp3 tracks as well as any addition style options as opts

```Javascript
<Playlist tracks={tracks} opts={playlistOverideStylingOpts}/>
```

## Screenshots

_Desktop_
![Alt text](public/Desktop.png)

_Desktop Hidden_
![Alt text](public/Desktop-hidden.png)

_Mobile_
![Alt text](public/Mobile.png)

_Mobile Hidden_
![Alt text](public/Mobile-hidden.png)

## Adding new features to the mp3

Make any changes or additional features in the Player.js component and update the version (in the package.json) by 0.0.1 and then push all your changes to the repo.

### Publish to NPM

Firstly make sure to build to the dist folder. Run

```shell
yarn build
```

Then publish the update to npm by running

```shell
npm publish
```

Your update should now be live on NPM. Make sure to update the package in your project by running

```shell
yarn upgrade react-mp3-player
```

## Contributing

Download the repo to your machine

```shell
git clone https://github.com/in-touch-dev/intouch-mp3-player
```

Then to get up and running with a dev environment

In the project directory, you can run:

```shell
yarn start
```

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

```shell
yarn test
```

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

```shell
yarn run build
```

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

```shell
yarn run eject
```

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

### Contributors

Liam Riley - github.com/Liamriley123
Dannish Hussain - github.com/Dannish94
Austin Kershaw - github.com/austinmkershaw
