# Parking_Project
this project will implement a parking circut in verilog. this praking can hold up to 700 cars and is opened at 8am.this parking priotizies the university staff.

![_smart-systems-parking-management-solid-color-background-4k-ultra-hd_964851-139576.avif](https://github.com/sepehrzoli/Parking_Project/blob/main/smart-systems-parking-management-solid-color-background-4k-ultra-hd_964851-139576.avif)

# Parking managment

Our Project is a parking mananger that can manage the specified parking in the description.


## Tools
- Verilog (Using its reg and wire)

## Implementation Details
  it has 5 major steps:
- 1.Define the module for parking management.
-  2.Use registers and counters for total spaces (700) and available staff/visitor spaces.
-    3.Implement priority logic to allocate spots to staff first, then visitors.
-    4.Use sensors and flags to detect car presence and update counters.
-    5.Generate output signals to display available spots for staff and visitors.


## Module Ports
### Inputs
- car_entered: shows that if a car has came to the parking.
- is_uni_car_entered: is the entered car, for the staff?
- car_exited: shows that if a car has exited the parking.
- is_uni_car_exited: is the exited car, for the staff?
- c_time : shows the hour of the current time. it's 5 bits to fit 24 numbers.

### Outputs
- uni_parked_car: number of parked cars that are for the staff.
- parked_car: number of parked cars that are not for the staff.
- uni_vacated_space: number of empty spaces for the staff.
- vacated_space: number of empty spaces for the non-staff.
- uni_is_vacated_space: is there any space for the staff?
- is_vacated_space: is there any space for the non-staff?

## Testing and What i did
for testing, because it's a very big test, we can't show it here, and it is in the documentation and the code, but i give a quick recap:because we want to test the code for edge cases and all the possible cases, we can't be sure of that we tested all the possible outcomes, so , first, by a for , we insert 400 cars to the parking, then , we write a python code that generates all the possible incoming cars, for a arbitary number of cars.so , by generating a test at random, we can be sure that we tested all the outcomes, and you can see the outcomes by runnig the code because it is about 1000 lines!!(it is very complete and thought-through).
## Authors
- [Sepehr Zolfaghari](https://github.com/sepehrzoli)

