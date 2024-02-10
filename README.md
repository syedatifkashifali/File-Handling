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
