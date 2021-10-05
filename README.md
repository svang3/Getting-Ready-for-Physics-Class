# Getting-Ready-for-Physics-Class

# Uncomment this when you reach the "Use the Force" section
train_mass = 22680
train_acceleration = 10
train_distance = 100
bomb_mass = 1

# Turn up the Temperature

# create a function to calculate Fahrenheit to Celsius.
def f_to_c(f_temp):
  c_temp = (f_temp - 32) * 5/9
  return c_temp

# test out function
f100_in_celsius = f_to_c(100)
print(f100_in_celsius)

# create a function to calculate Celsius to Fahrenheit.
def c_to_f(c_temp):
  f_temp = c_temp * (9/5) + 32
  return f_temp

# test out function
c0_in_fahrenheit = c_to_f(0)
print(c0_in_fahrenheit)

# Use the Force

# create a function to calculate the force.
def get_force(mass, acceleration):
  return mass*acceleration

# test out the function
train_force = get_force(train_mass, train_acceleration)
print(train_force)

# print sentence using train force
print("The GE train supplies " + str(train_force) + " Newtons of force.")

# create function to calculate the energy.
def get_energy(mass, c = 3*10**8):
  return mass*c

# test out the function
bomb_energy = get_energy(bomb_mass)

# print sentence using bomb energy
print("A 1kg bomb supplies " + str(bomb_energy) + " Joules.")

# Do the Work

# create function to calculate the work
def get_work(mass, acceleration, distance):
  return get_force(mass, acceleration) * distance

# test out the function
train_work = get_work(train_mass, train_acceleration, train_distance)

# print sentence using train work
print("The GE train does " + str(train_work) + " Joules of work over " + str(train_distance) + " meters.")
