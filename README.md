# Transfer-0.-...-in-0.-010101
This script transfer a fraction number based on 10 to get a fraction number based on 2.
_______________________________________________________________________________
Transfer 0. ... in 0. 010101
code:
_______________________________________________________________________________
a1 = float(input('Write a fraction number 0. ... based on 10 to get a fraction number based on 2\n'))
ansFr = []
for i in range(50):
    if i == 0:
        a2 = a1*2
    else:
        a2 = a2*2
    if a2 < 1:
        ansFr.extend([0])
    elif a2 > 1:
        a2 = a2 - 1
        ansFr.extend([1])
    elif a2 == 1:
        ansFr.extend([1])
        break
map(str, ansFr)
print(' '.join(map(str, ansFr)))
print('This number has 0. ... (50). ( numbers after sign , )')
