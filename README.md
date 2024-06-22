chocolate=list(map(int,input("enter the number of chocolates in the jars").split()))
N=len(chocolate)
count=0
for i in chocolate:
        if i==0:
            continue
        if i<=3:
            count=count+1
        else:
            if i%3==0:
                count=count+(i//3)
            else:
                count=count+(i//3)+1
print(count)
