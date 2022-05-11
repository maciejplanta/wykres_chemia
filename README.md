
import numpy as np
import matplotlib.pyplot as plt
import pylab



%matplotlib notebook


okno=plt.figure(figsize=(6,5), dpi=100, facecolor='lightgreen')


x=np.arange(1,21)
y1 = (1312,2372,521,899,801,1087,1402,1313,1681,2081,496,737,577,786,1011,999,1251,1520,418,589)
y2 = (x+1250)


plt.xlabel('Liczba Atomowa Z')
plt.ylabel('energia jonizacji [kJ/mol]')


plt.plot(np.linspace(1,0,1))
zmienna= plt.text(.99,1250,'H',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(1.99,2357,'He',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(2.94,518,'Li',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(3.98,958,'Be',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(5.00,733,'B',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(6.06,1128,'C',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(6.96,1412,'N',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(8.00,1299,'O',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(9.09,1730,'F',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(10.20,2090,'Ne',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(11.09,496,'Na',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(11.93,741,'Mg',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(12.92,572,'Al',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(14.23,857,'Si',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(14.96,1015,'P',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(16.09,992,'S',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(17.18,1331,'Cl',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(18.01,1520,'Ar',alpha=1)
zmienna.set_bbox(dict(facecolor='yellow', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(18.99,409,'K',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))

plt.plot(np.linspace(0,0,0))
zmienna = plt.text(20.07,594,'Ca',alpha=1)
zmienna.set_bbox(dict(facecolor='lightblue', alpha=1, edgecolor='red'))


plt.axvline(x=2,color="black",ls='--')


plt.axvline(x=10,color="black",ls='--')

plt.axvline(x=18,color="black",ls='--')


plt.title('zależność energii joniazacji w[kJ/mol] od liczby atomowej Z ')


plt.plot(x,y1,lw=1.5,color="red",label='EJ(Z)')


plt.plot(x,y2,lw=1.5,color="blue",label='Średnia energia jonizacji',ls='--')


plt.legend()


plt.grid()


#plt.savefig('C://Users//Maciek//Desktop//zaliczenie.pdf')
#plt.savefig('C://Users//Maciek//Desktop//zaliczenie.jpg')


pylab.show()
