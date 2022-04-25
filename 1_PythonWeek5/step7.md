# Python Week 5 Solutions

## Creating Classes
### DIY Task 
```
class Car():
    model = "BMW"
    passengers = 4
    colour = "red"
    speed = 5

    def calculate_acceleration(self):
        speed = speed + 2
        print(speed)
```

## Creating objects from a class
### DIY Task - Basic (Car)
```
class Car(object):
    def __init__(self, model, passengers, colour, speed):
        self.car_type = model
        self.max_passengers = passengers
        self.colour = colour
        self.speed = speed

    def get_car_data(self):
        list = [self.car_type, self.max_passengers, self.colour, self.speed, self.top_speed]
        return list

    def calculate_acceleration(self):
        self.speed = self.speed + 2
        print (self.speed)
```
### DIY Task - Advanced (Car)
```
class Car(object):
    def __init__(self, car, ppl, paint, current_speed, max_speed, cost):
        self.car_type = car
        self.max_passengers = ppl
        self.colour = paint
        self.speed = current_speed
        self.top_speed = max_speed
        self.price = cost

    def get_car_data(self):
        list = [self.car_type, self.max_passengers, self.colour, self.speed, self.top_speed]
        print("""Car Model: %s
Maximum Number of Passengers: %s
Colour of Car: %s
Maximum Speed: %s
Price: %s""" % (self.car_type, self.max_passengers, self.colour, self.speed, self.top_speed))
        return list

    def calculate_acceleration(self):
        self.speed = self.speed + 2
        print (self.speed)
