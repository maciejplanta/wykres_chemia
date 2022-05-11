# Dodanie poszczególnych bibliotek do analizy wizualnej
import numpy as np
import matplotlib.pyplot as plt
import pylab


# matplotlib notebook umożliwia rysowanie w notatniku jupyter.
%matplotlib notebook

# okno wykresu. figsize oznacza rozmiary czyli długość i szerokość wykresu, dpi - rozdzielczość, facecolor - kolor zła
okno=plt.figure(figsize=(6,5), dpi=100, facecolor='lightgreen')

# stworzenie listy zmiennych x,y1,y2
x=np.arange(1,21)
y1 = (1312,2372,521,899,801,1087,1402,1313,1681,2081,496,737,577,786,1011,999,1251,1520,418,589)
y2 = (x+1250)

# dodanie nazw osi xlabel - nazwa osi x, ylabel - nazwa osi y
plt.xlabel('Liczba Atomowa Z')
plt.ylabel('energia jonizacji [kJ/mol]')

# linespace zwraca równomiernie rozmieszczone liczby w określonym przedziale.
# plt.text położenie x i y na wykresie
# transaxes czyli koordynaty układu współrzędnych,
# alpha - intensywność czcionki, facecolor- kolor tła, edgecolor - kolor obramowania
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

# axvline - pionowa linia dla zmiennej x=1, ls- rodzaj linii - przerywany (linia wertykalna - pionowa)
plt.axvline(x=2,color="black",ls='--')

# jw. dla x=9
plt.axvline(x=10,color="black",ls='--')

# jw. dla x=17
plt.axvline(x=18,color="black",ls='--')

# plt.title - tytuł wykresu
plt.title('zależność energii joniazacji w[kJ/mol] od liczby atomowej Z ')

# dane wprowadzone dla x i y1 powyżej, label - tytuł(pokazuje się w legend(), lw - grubość linii)
plt.plot(x,y1,lw=1.5,color="red",label='EJ(Z)')

# jw dla innych danych
plt.plot(x,y2,lw=1.5,color="blue",label='Średnia energia jonizacji',ls='--')

# legenda
plt.legend()

# siatkowanie
plt.grid()
# zapis na komputerze

#plt.savefig('C://Users//Maciek//Desktop//zaliczenie.pdf')
#plt.savefig('C://Users//Maciek//Desktop//zaliczenie.jpg')

# pokaz wyniki(może być nie musi)
pylab.show()
