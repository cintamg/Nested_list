# Nested_list
To find the second lowest scorer in a list.
if __name__ == '__main__':
    n=int(input())
    marksheet=[]
    marksheet=[[input(),float(input())]for _ in range(n)]
    second_highest=sorted(list(set(marks for name,marks in marksheet)))[1]
    print('\n'.join([a for a,b in sorted(marksheet) if b==second_highest]))
