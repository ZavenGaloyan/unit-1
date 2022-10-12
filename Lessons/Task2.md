Task was to create a program for an EV calculator. A given set of data was provided and parameters for calcuations that were needed to be completed
Below is the data and code for the Program

Date,Charge,Duration                                                                                                                                                   .
12.9.22,8.878kWh,12:32:36
15.9.22,3.533kWh,5:02:23
17.9.22,6.828kWh,9:41:46
18.9.22,5.425kWh,7:43:35

```.py
from My_library import validate_int_input, end_code, green, bold_green

Welcome_msg = "Welcome to the EV Calculater".center(50,"=")
prompt_msg = "Please enter an option:"
print(f"{green}{Welcome_msg}{end_code}")
print("Options".center(50))

menu = """1. Average time per kWh
2. Total kwh
3. Total charge time
4 Show all data
"""

print(menu)
option = validate_int_input(prompt_msg)
while option>4 or option < 1:
    option = validate_int_input(f"{green}Invalid option. {prompt_msg}{end_code}")

with open ("Charging_log.csv", "r") as file:
    ev_logs = file.readlines()

if option == 4:
    print(f"{bold_green}4. Showing all data{end_code}")
    index = 0
    for log in ev_logs:
          if index>0:
             print(f"{bold_green}No.{index}:{log}{end_code}")
          index += 1

if option == 2:
    index = 0
    total_energy = 0
    for log in ev_logs:
          if index>0:
              values = log.split(",")
              date = values[0]
              energy = values[1]
              time = values[2]
              total_energy += float(energy[0:5])
          index += 1
    print(f"{green}The total energy charged is {total_energy} Kwh")

if option == 3:
    index = 0
    total_time1 = 0
    total_time2 = 0
    total_time3 = 0
    for log in ev_logs:
          if index>0:
              sec = log.split(":")
              hour = sec[0]
              minute = sec[1]
              second =sec [2]
              total_time1 += float(hour[16:18])
              total_time2 += float(minute[0:2])
              total_time3 += float(second[0:2])
          index += 1

    print(f"{green}The total energy charged is {total_time1}:{total_time2}:{total_time3}")
