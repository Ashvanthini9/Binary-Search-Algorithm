# Binary-Search-Algorithm

    def binarySearch(arr,first,last,item):  
        if last >= first:  
            mid = int((first+last)/2)  
            if arr[mid] == item :  
                return mid
            elif arr[mid] < item :   
                return binarySearch(arr,mid+1,last,item)  
            else:   
                return binarySearch(arr,first,mid-1,item)  
        return -1  


    arr=[16, 19, 20, 23, 45, 56, 78, 90, 96, 100];  
    item = int(input("Enter the item which you want to search ?"))  
    location = -1;   
    location = binarySearch(arr,0,9,item);  
    if location != -1:   
        print("Item found at location %d" %(location))  
    else:   
        print("Item not found") 
