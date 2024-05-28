## README

# Ruby on Rails 3.3.1 Pet Tracker API App

### 1. Download source code and run app
   
https://github.com/Overbrd/ruby-on-rails-pet-tracker-app

Open folder in Node

Run this command to start server: rails server

### 2. Use Postman to Test
   
Open Postman and create a new GET request

Use this URL for the GET request: localhost:3000/owners/:id/pets

Use this setting

Under Params->Path Variable->id->value

Use this id 1 (or 2)

Press Send

You will see 200 OK status and output will be the data based on the id you used above.

## additional commands...

### 1. create a new POST request to create a new Owner:

Choose “POST” from the dropdown on the left, and enter localhost:3000/owners as the request URL

navigate to the Body tab, choose raw, and select JSON from the dropdown on the right. Add the following code to the request body:

```
{
"name": "put a name here",
"email": "put a email address here"
}
```

Press Send

You will see 200 OK status and output will be the data you input above.

Repeat steps above and input a second entry of dummy data to create a second owner.

### 2. create a new POST request to create a new Pet:

Choose “POST” from the dropdown on the left, and enter localhost:3000/pets as the request URL

navigate to the Body tab, choose raw, and select JSON from the dropdown on the right. Add the following code to the request body:

```
{
"name": "put a name here",
"species": "put a species here",
"breed": "put a breed here",
"age": put an age here,
"owner_id": put a number here (other than 1 or 2)
}
```

Press Send

You will see 200 OK status and output will be the data you input above.




