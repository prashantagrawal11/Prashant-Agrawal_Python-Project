# Prashant-Agrawal_Python-Project
#taking input from the user in form of list
list=[s for s in input("Enter strings: ").split(',')]
print('Input list:',list)
#defining function
def acronym(Str):
    #Fetching all strings
    a = Str.split()
    output = ""
    #iterating over words
    for i in a:
        output += i[0]
    #capitalising output
    output = output.upper()
    return output
out=[]
#iterating over input list containing strings
for i in list:
    #calling function and storing output in list
    out.append(acronym(i))
#printing output
print('Output Acronym list:',out)
