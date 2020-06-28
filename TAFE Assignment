from datetime import date
today = date.today()

# access the confpack text file and read the records into an array
confPackArray = []
with open('confPack.txt') as f:
    for line in f:
        inner_list = [elt.strip() for elt in line.split(',')]
        confPackArray.append(inner_list)

Basic = confPackArray[0]
Bonus = confPackArray[-1]

# access the employees text file and loop through the records (checking for the end of file)
# use logical operators to select the appropriate conference attendees
# display the required information.

def check():
    with open('employees.txt') as f:
        data = f.read()
        
    employee_line = data.split('\n', 5)[3][-3:]
    print(employee_line) # Code here checks last 3 elements of employees.txt line 4 (Kline,Bob,Y,Y)
    employee_name = data.split('\n', 5)[3]
    print(employee_name) # Code here is to pull out employee Surname and First Name (NOT the Y,Y on the end)

    if "Y" and "Y" in employee_line:
        return True
    elif "Y" in employee_line:
        return True
    else:
        return False
    
if check():
    print('True')
else:
    print('False')

# Print Report date: [dd/mm/yyyy]
d1 = today.strftime("%d/%m/%Y")
print("Report Date:", d1)

# Final goal is to print to IDE terminal the following information (formatted as shown below)
# Attendee: [Surname, first name] Pack/s: [1 or 2 days pack], [both days pack]
