# Nouns 
---- 


## Location 
This the place of something 
### Attribtes (property)
- `Location.latitude`
  - variable_type: `float` 
  - required: y 
- `Location.longitude` 
  - variable_type: `float` 
  - required: y 
### Data Source 
----
## Trail (Hannah)
### Attributes 
- `Trail.traffic_current` 
  - description: describes the amount of traffic at a particular trail, at current hour 
  - method_type: instance 
  - params: traffic api source
  - return: an array of string (low, medium, high traffic) and an integer of current traffic
- `Trail.traffic_average_all_time` 
  - description: describes the average amount of traffic at a trail over time 
  - method_type: instance 
  - params: [:traffic_data, array]
  - return: float of average overall traffic 
- `Trail.traffic_average_per_hour(day)` 
  - description: returns an array of traffic levels at every hour of the day (index:0=> 1:00am, index:2 => 2:00am)
  - method_type: instance
  - params: [:hour, integer]
  - return: hash of time pointing to traffic integer 
- `Trail.type` 
  - description: defines what activities are at that trail instance 
  - method_type: instance
  - params: trail.all.find_by(params[:activities])
  - return: array of strings
- `Trail.length` 
  - description: defines how long the trail is in miles/kilometers 
  - method_type: instance
  - params: trail.all.find_by(params[:length])
  - return: float
- `Trail.shade_level` 
  - description: defines the relative amount of shade on a scale. 
  - method_type: instance
  - params:
  - return: string
- `Trail.pets_allowed` 
  - description: returns the types of pets allowed (`nil` if no pets allowed)
  - method_type: instance
  - returns: Array[Pets]
- `Trail.info`
  - description: calls on prior methods to view all the info for that trail and displays it
  - method_type: instance
  - params:
  - return: A string that includes all the data from the methods called
### Methods
- `` 
--- 
## User (Lisa)
### Attributes (characteristics)
- `Class.username`
  - description: the users chosen name 
  - attribute_type:
- `Class.first_name`
  - description: the given name of a user
  - attribute_type:  
### Methods (verb)
- `Class.method`
  - description:" 
  - method_type: [instance/class] 
  - params: [name:string, age:integer]
  - return: name 
### Data Source 
  - where is the information coming from 
---- 
## Hike (Jason)
### Attributes (characteristics)
- `Class.attribute`
  - description: 
  - method_type:  
### Methods (verb)
- `Class.attribute`
  - description:" 
  - method_type: [instance/class] 
  - params: [name:string, age:integer]
  - return: name 
### Data Source 
  - where is the information coming from 
---- 

 
-----
--> Down the line (v2)
---- 
## Mountain 
Represent a physical mountain 
### Attribtes (property)
- `Mountain.name` 
  - method_type: `instance`
- `Mountain.location` 
  - description: returns location 
  - method_type: `instance` 
  - return: `Location` 
- `Mountain.all`
  - description: returns all mountain records
  - method_type: `class` (self.all)
  - return: [Mountains]

### Methods (verb)
- `Mountain.findClosest()` 
  - class: `Mountain` 
  - description: finds the nearest mountain related to the object called upon
  - method_type: `instance` 
  - params: `nil`
  - return: `Array[Mountains]
### Data Source 
---- 
## Conditions 
---- 
## Equipment 
---- 
## Parking 
### Attributes
- `Parking.spots_available` 
### Methods (verb)
- `Class.attribute`
  - description:" 
  - method_type: [instance/class] 
  - params: [name:string, age:integer]
  - return: name 
---- 



> Template 
---- 
## Object_Name 
### Attributes (characteristics)
- `Class.attribute`
  - description: 
  - method_type:  
### Methods (verb)
- `Class.attribute`
  - description:" 
  - method_type: [instance/class] 
  - params: [name:string, age:integer]
  - return: name 
### Data Source 
  - where is the information coming from 
--- 
