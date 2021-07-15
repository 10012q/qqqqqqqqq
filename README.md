import math
record_in_seconds = float(input())
distans_in_meters = float(input())
time_for_one_meter = float(input())

swiming_needs = distans_in_meters*time_for_one_meter
after_15_meters = math.floor((distans_in_meters/15)) * 12.5
sum_time = swiming_needs + after_15_meters
if record_in_seconds > sum_time:
    print(f"Yes, he succeeded! The new world record is {sum_time:.2f} seconds.")
else:
    
    print(f"No, he failed! He was {sum_time-record_in_seconds:.2f} seconds slower.")
