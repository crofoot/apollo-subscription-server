# apollo-subscription-server
> Example of Apollo Subscription Server

### Setup
* first clone `apollo-subscription-server`
* `npm install`
* `npm start`


### Usage
* open http://localhost:4000/graphql
* In the first tab start the subscription query 
```
subscription {
  subscribeToNotifications{
    message
    date
    title
  }
}
```
* In another tab send the following mutation. Go back to original tab and you should see the message and date popup in the apollo console

```
mutation {
  createNotification(message: "Hello" title: "Alert for you!")
}

```