# Spring boot with kafka

The project will allow you to publish messages into a kafka topic using a spring boot producer and consume messages from the same topic and display it into the console

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

java 8+
kafka must be up and running before starting the app
create a topic `users`



### Installing

git clone or download the project

import the project in your favourite IDE

run the zookeeper first

run kafka

run the app
## Testing

Send a post request to : http://localhost:9000/kafka/publish?message=`the message you want to publish`

If you see your message on the console then it is working
## Explanation
The controller is receiving publish requests from the client and forwording them to the producer.
The producer writes the message in the `users` topic 
The consumer reads the message from the topic and display it on the console