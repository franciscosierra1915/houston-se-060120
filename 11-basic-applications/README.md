# CLI Applications

### Learning Goals

- Plan and scope the development of an application
- Use TTY Prompt to get data from the user 
- Use RestClient to get data from the internet

### Planning

###### User Stories
* As a user I can see my tickets
* As a user I can purchase a ticket
    * With a seat
* See other passengers who flew with the same airline
* Cancel a ticket


##### MVP
* As a user I can purchase a ticket
* As a user I can see my tickets

##### Stretch Goals
* See other passengers who flew with the same airline
* As a user I can purchase a ticket
    * With a seat
* Cancel a ticket
* Edit an airline

### Vocabulary
* CLI
    * An application that's run from the terminal
* User Story
    * "As a user, can do: _"
* MVP
    * Minimum Viable Product (features we need)
* Stretch Goal
    * Features we would like
* TTYPrompt
    * A gem which helps us build pretty interfaces
* API
    * A way to get data through the internet
* RestClient
    * A gem which helps us ask for data from the internet

<br>
<br>


```
response = RestClient.get("https://aviation-edge.com/v2/public/airlineDatabase?key=fcffba-1d4753")
airlines = JSON.parse(response.body)

airlines.each do | airline | 
    Airline.create({
        name: airline["nameAirline"],
        established: airline["founding"]
    })
end
```



```
ActiveRecord::Base.logger = nil
prompt = TTY::Prompt.new

# %w(Scorpion Kano Jax) === [ "Scorpion", "Kano", "Jax"]

a = Artii::Base.new :font => 'slant'
prompt.say(a.asciify('Airlines'))
```

