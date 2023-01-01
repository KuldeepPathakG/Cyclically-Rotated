# Cyclically-Rotated

def rotate(A,n):
    x=A[n-1]
    for i in range(n-1,0,-1):
        A[i]= A[i-1]
    A[0]= x

arr=[1, 2, 3, 4, 5]
print("Original Array: ",arr)
n=len(arr)
for i in range(0,n):
    print(arr[i], end="")
rotate(arr,n)
print("\n Rotated Array: ")
for i in range(0,n):
    print(arr[i], end="")
