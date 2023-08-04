# helloCR
#finding second runner-up in a list by HackersRank.
if __name__ == '__main__':
    n=int(input())
    list1=list(map(int,input().split(" ")))
    arr=list(set(list1))
    c=arr.count(max(arr))
    for i in range(n):
        if i==c:
            i+=1
            arr.sort()
    print(arr[-2])
