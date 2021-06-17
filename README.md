##Redux
Redux is an open-source JavaScript library for managing application state.

##Why I Study Redux
If we do not use Redux, several components use "props" to send and receive data directly and use each of them. If this method is used, a problem arises in that when one component needs to be deleted or modified, other related components must also be modified. This problem is not a big deal for small applications, but if the size of the application grows, the logic of the code will become very complex.

On the other hand, if we use Redux, we form a centralized system centered on “store” and disconnect between each component. Each component "dispatch" the "action" containing the change of its own "state" to the "store", and then change the original "state" through the "reducer". Also, when the original "state" is changed, other components "subscribed" to the "store" are notified. The notified components use "getState" to get the value of "state" and then render. After all, when we use Redux, we can change components without direct connection between each component.

As Redux guarantees the independence of components, it lowers the dependency between components and makes maintenance easier.

##Reference
https://github.com/reduxjs/redux
https://redux.js.org/api/store

