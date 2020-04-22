# Overtime-prediction-
Program to calculate any over time 

promptHours = 'Please enter your hours you have worked '
try:
    hours = float(input(promptHours))
except:
    print('please enter a number!')
    
    
PromptHourlyrate = 'Please enter your hourly rate '
try:
    rate = float(input(PromptHourlyrate))
except:
    print('please enter a number!')
    
    if hours <= 40:
    pay = (rate) * (hours)
    print(pay)   
elif hours > 40:
    overtimePay =((hours - 40)*rate*1.5)+rate*40
    print(overtimePay)
