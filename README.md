# File-Handling 


#creating file using python
f=open('new.txt','w')
f.write("Bano-Qabil")
f.close()

#reading file using python
f=open('new.txt')
print(f.read())
f.close()

#appending in file using python
f=open('new.txt','a')
f.write("\nSo practice it daily")
f=open('new.txt')
print(f.read())

#reading file line by line 
f=open('new.txt')
print(f.readline())#printing first line
print(f.readline())#printing line after

#creating csv file
import csv
with open('protagonist.csv', 'w', newline='') as file:
    writer = csv.writer(file)
    writer.writerow(["SN", "Movie", "Protagonist"])
    writer.writerow([1, "Lord of the Rings", "Frodo Baggins"])
    writer.writerow([2, "Harry Potter", "Harry Potter"])


#reading csv file
import csv

with open('people.csv', 'r') as file:
    reader = csv.reader(file)

    for row in reader:
        print(row)

#manipulating data in csv file
import csv
with open("aaa.csv","w") as x:
	file=csv.writer(x)
	for i in range(1, 6):
		sr=input("enter serial number")
		data=input("enter data")
		file.writerow([sr,data])
	x.close()
