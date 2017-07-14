# This project is based on Amazon Voice Server

# It's a Spring-boot project


You can test in this way

#### Intent Schema
```json
{
	"intents": [
		{
			"intent": "Hello",
			"slots": []
		},
		{
			"intent": "HelloMe",
			"slots": [
				{
					"name": "Who",
					"type": "AMAZON.US_FIRST_NAME"
				}
			]
		},
		{
			"intent": "Add",
			"slots": [
				{
					"name": "NumberA",
					"type": "AMAZON.NUMBER"
				},
				{
					"name": "NumberB",
					"type": "AMAZON.NUMBER"
				}
			]
		}
	]
}
```

#### Sample Utterances
```text
Hello Hello
Hello Hi
Hello Hi There
Hello What's Up
Hello Howdy

HelloMe I am {Who}
HelloMe This is {Who}

Add Add {NumberA} and {NumberB}
Add Sum {NumberA} and {NumberB}
```


Use the following to test the 3 intents configured 

1. hi (should return you Welcome)

1. i am peru (should return Welcome Peru)

1. add twelve and thirteen (should return The sum of the two numbers are 25)