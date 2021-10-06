# To print a bingo table
import random
one=[1,2,3,4,5]
two=[6,7,8,9,10]
three=[11,12,13,14,15]
four=[16,17,18,19,20]
five=[21,22,23,24,25]

li1=[]
random.shuffle(one)
for i in one:
    li1.append(i)
li2=[]
random.shuffle(two)
for i in two:
    li2.append(i) 
li3=[]
random.shuffle(three)
for i in three:
    li3.append(i)   
li4=[]
random.shuffle(four)
for i in four:
    li4.append(i)  
li5=[]
random.shuffle(five)
for i in five:
    li5.append(i)    


#print("Enter the table\n")

'''li1=[int(x) for x in input().split()]
li2=[int(x) for x in input().split()]
li3=[int(x) for x in input().split()]
li4=[int(x) for x in input().split()]
li5=[int(x) for x in input().split()]'''

k=chr(10062)+"  "
def row(li):
    s=""
    for i in li:
        if i==chr(10062):
            s+=k
            #s+=" "
        elif i<10:
            s+=str(i)
            s+=" "*2
        else:
            s+=str(i)
            s+=" "*1
    print(s)
print("\nBingo Table\n")
print("Let's Start..\n")

# To show the table every time 
def show():
    row(li1)
    row(li2)
    row(li3)
    row(li4)
    row(li5)
show()    


#to strike the value in the table

def strike(li1,li2,li3,li4,li5,n):
    if(n in li1):   li1[li1.index(n)]=chr(10062)
    elif(n in li2): li2[li2.index(n)]=chr(10062)
    elif(n in li3): li3[li3.index(n)]=chr(10062)
    elif(n in li4): li4[li4.index(n)]=chr(10062)
    elif(n in li5): li5[li5.index(n)]=chr(10062)
    show()
#strike(li1,li2,li3,li4,li5,n) 

#to check whether any matches found
def check(li):
    c=0
    for i in li:
        if i==chr(10062):
            c+=1
    if c==5:
        return True
        
bingo=0
r1,r2,r3,r4,r5=0,0,0,0,0
c1,c2,c3,c4,c5=0,0,0,0,0
d1,d2=0,0
while(bingo<5):
    n=int(input("\nEnter the value\t"))
    strike(li1,li2,li3,li4,li5,n)
    if r1==0:
        if(check(li1)):
            bingo+=1
            r1+=1
            print(bingo," OVER...")
    if r2==0:
        if(check(li2)):
            bingo+=1
            r2+=1
            print(bingo," OVER...")
    if r3==0:
        if(check(li3)):
            bingo+=1
            r3+=1 
            print(bingo," OVER...")
    if r4==0:
        if(check(li4)):
            bingo+=1
            r4+=1 
            print(bingo," OVER...")
    if r5==0:
        if(check(li5)):
            bingo+=1
            r5+=1 
            print(bingo," OVER...")
    if c1==0:
        col1=[li1[0],li2[0],li3[0],li4[0],li5[0]]
        if(check(col1)):
            bingo+=1
            c1+=1
            print(bingo," OVER...")
    if c2==0:
        col2=[li1[1],li2[1],li3[1],li4[1],li5[1]]
        if(check(col2)):
            bingo+=1
            c2+=1
            print(bingo," OVER...")
    if c3==0:
        col3=[li1[2],li2[2],li3[2],li4[2],li5[2]]
        if(check(col3)):
            bingo+=1
            c3+=1  
            print(bingo," OVER...")
    if c4==0:
        col4=[li1[3],li2[3],li3[3],li4[3],li5[3]]
        if(check(col4)):
            bingo+=1
            c4+=1   
            print(bingo," OVER...")
    if c5==0:
        col5=[li1[4],li2[4],li3[4],li4[4],li5[4]]
        if(check(col5)):
            bingo+=1
            c5+=1
            print(bingo," OVER...")
    if d1==0:
        digoanl1=[li1[0],li2[1],li3[2],li4[3],li5[4]]
        if(check(digoanl1)):
            bingo+=1
            d1+=1
            print(bingo," OVER...")
    if d2==0:
        digoanl2=[li1[4],li2[3],li3[2],li4[1],li5[0]]
        if(check(digoanl2)):
            bingo+=1
            d2+=1
            print(bingo," OVER...")

if bingo==5:
    print("\n\t BINGO! \n\t GAME OVER!")
 
