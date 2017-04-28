# Randomizer
Development of Rest endpoint

### List of endpoints:

##### /distributions/randoms

|Method|Result|
|----------------------|----------------------|
|GET   |Return list of randomly generated numbers|
|PUT   |Update default generator|

###### GET
Returns a json list of numbers which are randomly generated using the normal distribution. 
Call can be made using the following:

http://127.0.0.1/rest/distributions/randoms

__Parameters__

|Parameter|Required|Result|
|----------------------|----------------------|
|num1|no|A number used to allow for randomly generated numbers between 2 points|
|num2|no|The second number for randomly geerated numbers between 2 points|
|limit|yes|The amount of randomly generated number your wish to receive|
|offset|no|Used to page through results|


###### PUT
Allows you to update the deafult generator when using the endpoint. 
Call can be made using the following:

http://127.0.0.1/rest/distributions/randoms

{
    "generator": "-batch-"       // new generator
}

__Generators__
1. -batch- = Return multiple random numbers
2. -single- = Return single random number (Default)

##### /distributions/parabolas

|Method|Result|
|----------------------|----------------------|
|GET   |Return list of prabola generated numbers|
|PUT   |Update default parameter|

__generators__
1. -batch- = Return multiple random numbers
2. -single- = Return single random number (Default)
