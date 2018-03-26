# madzik
Python
def hotel_cost(days):
  return 140 * days

def plane_ride_cost(city):
  if city == “Victoria Falls”:
    return 183
  elif city == "Bulawayo":
    return 220
  elif city == "Johannesburg":
    return 222
  elif city == "Lusaka":
    return 475

def rental_car_cost(days):
  cost = days * 40
  if days >= 7:
    cost -= 50
  elif days >= 3:
    cost -= 20
  return cost


def trip_cost(city, days, spending_money):
  return hotel_cost(days) + plane_ride_cost(city) + rental_car_cost(days) + spending_money

print trip_cost("Victoria Falls", 5, 600)
