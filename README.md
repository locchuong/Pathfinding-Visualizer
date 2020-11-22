# Pathfinding Visualizer
A simple pathfinding visualizer built on react. I made this app while learning to work with react so I may have commited some react crimes, but hopefully someone will provide some insight on this; I'm open to criticism. If you'd like to try this web app out, feel free to access it [here](https://pathfinding-visualizer-react.herokuapp.com/). Additionally, feel free to fork this if you'd like to base your projects off this, I had a lot of fun creating this project. A special thanks to Clement Mihailescu for his youtube tutorial which introducted me to working with react.

## Algorithms
**Dijkstra's Algorithm**: Developed by Edsger W. DIjkstra, this algorithm guarantees the shortest path between two nodes in a graph. It does so by repeatedly expanding the closest vertex which has not been visited in conjunction with a priority queue of distance values from the start node. Note that this algorithm is weighted.

**Breath-first Search**: This algorithm guarantees the shortest path between two nodes in a graph by exporting all neighbor nodes at the present depth prior to moving on to the next depth level of nodes. It does so using a queue as its data structure. Note that this algorithm is unweighted.

**Depth-first Search**: This algorithm does **not** guarantee a shortest path and is a terrible algorithm for pathfinding. DFS explores as far as possible along each "branch" before backtracking. While it does guarantee a path to the end node, it is almost always not the shortest path.

**A STAR Search Algorithm**: This algorithm is a graph traversal and path finding algorithm that guarantees the shortest path using heuristics to guide it. It does so by keeping track of a fcost, hcost and gcost where hcost is the projected distance from any given node to the end node and gcost is the distance to the start node. Fcost is simply hcost + gcost. The heuristic used in this implementation is Euclidean distance, but Manhattan distance is also implemented (commented out). The data structure used to implement this algorithm was a priority queue which orders the nodes by fcost.

**Recursive Subdivision**: This algorithm picks a random pivot point, creates a wall at the pivot with a random passages along it, and then recursively calls the algorithm on the subdivided regions. Because entire cells (Instead of the outline of the cells) were used as walls, walls are restricted to having even-numbered indices and passages are restricted to odd-numbered indices.

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
