# evenoddnums
numbers = input("Enter a list of numbers: ")
numlist = numbers.split()
for i in range(len(numlist)):
    numlist[i] = int(numlist[i])
    
def classify_numbers(numlist):
    evens = [ ]
    odds = [ ]
    for x in numlist:
        if x % 2 == 0:
            evens.append(x)
        else:
            odds.append(x)
    return evens, odds

evens, odds = classify_numbers(numlist)
print("Even numbers:", evens)
print("Odd numbers:", odds)
