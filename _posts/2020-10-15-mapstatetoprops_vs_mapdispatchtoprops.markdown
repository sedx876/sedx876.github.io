---
layout: post
title:      "mapStateToProps Vs. mapDispatchToProps"
date:       2020-10-15 19:53:13 +0000
permalink:  mapstatetoprops_vs_mapdispatchtoprops
---


React-Redux provides us two important functions in order to work with our state and props. They are `mapStateToProps` and `mapDispatchToProps`

On its most basic level...

`mapStateToProps` connects redux state to props of react component.

`mapDispatchToProps` connects redux actions to react props.

In our top level component(App), our export has a connect that is taking two arguments. The first argument is `mapStateToProps`. Our second is `mapDispatchToProps`. Both arguments are concerned with `currentUser`.

![enter image description here](https://i.ibb.co/QHzGftc/2020-10-15-14-37.png)

`mapStateToProps` is called every time the store state changes. It should return an object of data this component needs. We are asking our store about our `currentUser` and the data that is tied to it. We will hand off the state from our store to the component so we can work with the data.

![enter image description here](https://i.ibb.co/xDX8hmS/2020-10-15-14-42.png)

`mapDispatchToProps` is our second argument which in this case is an object. Now it has to find its `actionCreator`.

Since we previously imported our `getCurrentUser ` action at the top of our component, we can directly dispatch our action directly from our component to find the exact `actionCreator` we need.

![enter image description here](https://i.ibb.co/TMkcsfs/2020-10-15-15-17.png)

We find our action, which in this case is a `GET` request fetch to the backend to find our user.

![enter image description here](https://i.ibb.co/qFfd888/2020-10-15-15-22.png)

From here we will go to our `currentUser` reducer

![enter image description here](https://i.ibb.co/jHd490P/2020-10-15-15-39.png)


Reducer takes in state and action as arguments and then checks our case statement to tell our action how we are going to manage this state.

We then visit our store which is the gatekeeper to our state. It is in essence our traffic cop. It tells us where our state goes.

![enter image description here](https://i.ibb.co/XXSQ6ns/2020-10-15-15-45.png)

And finally we end up back in our component and we can map our state to our component props. It makes a nice neat circle (or diamond as illustrated in my crude graphic).
 
![enter image description here](https://i.ibb.co/Np7DLcC/2020-10-15-15-14.png)
