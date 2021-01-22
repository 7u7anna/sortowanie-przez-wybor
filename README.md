# sortowanie-przez-wybor
#metoda porzadkowana przez wybor
def choicemethod(T):
  n=len(T)
  for i in range(n-1):
    k=i
    for j in range(i+1,n):
      if T[j]>T[k]:
        k=j
    T[i] , T[k] = T[k] , T[i]
  return T

from random import randint 
T=[randint(1,100) for x in range(10)]
print(choicemethod(T))

#To jest wariant 1 i 2 poniewaz jak maleja od lewej to musza rosnac od prawej .
