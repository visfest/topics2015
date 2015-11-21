# D3 and React Sessions notes

## What is create? Why would I want to use it?

React takes care of the enter/update/exit boilerplate.
Someone mentioned they used react for their chatting app. "It's very explicit about introductin state"
"Hundreds of components, you have to be explicit about adding new state"
It does diffing for you so it runs very fast.
One thing about it is that it doesn't do transitions very well. Things jump from what state to another.
It might be helpful to talk about other frameworks to talk about what makes react special. In react, there's a concept of a uni-directional data flow. The state changes propigate now. That took a while for me to wrap my head around, but once I did, it make interacting with it a lot easier. For using React and D3, we'll put the D3 code into the `componentDidMount` lifecycle event. If things change, we'll hook that into `componentDidUpdate`.
I recently started using react for a side project. For us, the one of the most powerful features of react is server side rendering. Redux also works great for undo/redo functionality.
