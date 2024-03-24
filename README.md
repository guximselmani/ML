
# Pasqyrë e pergjithshme
Ky projekt zhvillohet si pjesë e kurrikulës së studimeve Master në Fakultetin e Inxhinierisë Elektrike dhe Kompjuterike në kuadër të lëndës 'Machine Learning'. Fokusohet në aspektet thelbësore të aplikimit të algoritmeve të ML në një domen të caktuar.

# Qëllimi
Objektivi kryesor i këtij projekti është të demonstrojë në përgjithësi përgatitjen, përpunimin dhe vizualizimin e të dhënave ashtu që të mund të zbatohen teknika dhe metodologji të ndryshme që lidhen me përgatitjen dhe krijimin e modelit parashikues dhe zbatimin e algoritmeve te ML.

# Hyrje
Ky dataset përmban një grup të të dhënave  për  makina të përdorura. Ai përfshin veçori të ndryshme të makinave si marka, modeli, viti, kilometrazhi, detajet e motorit, lloji i transmisionit, lloji i karburantit, çmimi, lëvizja dhe më shumë. Ai përfshin informacion mbi atributet e ndryshme të automjeteve dhe ndikimin e tyre, të cilat mund të përdoren për të marrë vendime të informuara në lidhje pronësine e automjetit. Pra qëllimi i këtij grupi të dhënash është të vlerësojë performancën e modeleve të mësimit të makinerive për të parashikuar nësë pronari i makinës, është apo nuk është pronari i parë i tij.

# Përshkrimi i datasetit
Dataseti i projektit është marrë nga Kaggle: 
https://www.kaggle.com/datasets/tugberkkaran/used-car-listings-features-and-prices-carscom

Ky dataset përmbanë 36 kolona:

1) Brand: Marka a makinës
2) Model: Modeli i makinës
3) Year: Viti i prodhimit të makinës
4) Mileage: Kilometrazhi i makinës
5) Engine: Informata mbi motorin e makinës
6) Engine_size: Informata mbi madhësinë e motorit
7) Transmission: Transmisioni i makinës
8) Automatic transmision: Ështē apo jo automatik
9) Fuel type: Lloji i karburantit
10) Drivetrain: Lloji i lëvizjes
11) Min_mpg: Efikasiteti minimal i karburantit të makinës
12) Max_mpg: Efikasiteti maksimal i karburantit të makinës
13) Damaged: Një vlerë binare që tregon praninë e dëmtimit në makinë (1: Po, 0: Jo)
14) First_owner: A është makina një automjet me 1 pronar? (1: Po, 0: Jo)
15) Personal_use: A është makina vetëm për përdorim personal? (1: Po, 0: Jo)
16) Turbo: Një vlerë binare që tregon praninë e një turbongarkuesi në makinë (1: Po, 0: Jo)
17) Alloy_wheels: A ka rrota aliazhi në makinë? (1: Po, 0: Jo)
18) Adaptive_cruise: Një vlerë binare që tregon praninë e kontrollit adaptiv (1: Po, 0: Jo)
19) Navigation_system: Një vlerë binare që tregon praninë e një sistemi navigimi (1: Po, 0: Jo)
20) Power_liftgate: Një vlerë binare që tregon praninë e një porta ngritëse elektrike (1: Po, 0: Jo)
21) Backup_camera: Një vlerë binare që tregon praninë e një kamere  (1: Po, 0: Jo)
22) Keyless_start: Një vlerë binare që tregon praninë e sistemit të startimit pa çelës (1: Po, 0: Jo)
23) Remote_start: Një vlerë binare që tregon praninë e një sistemi startimi në distancë (1: Po, 0: Jo)
24) Sunroof: Një vlerë binare që tregon praninë e një çati dielli/çati hëne (1: Po, 0: Jo)
25) Automatic_emergency_braking: Një vlerë binare që tregon praninë e sistemit automatik të frenimit emergjent (1: Po, 0: Jo)
26) Stability_control: Një vlerë binare që tregon praninë e sistemit të kontrollit të stabilitetit (1: Po, 0: Jo)
27) Leather_seats: A ka ulëse lëkure në makinë? (1: Po, 0: Jo)
28) Memory_seats: A ka vende memorie në makinë? (1: Po, 0: Jo)
29) Third_row_seating: Një vlerë binare që tregon praninë e ulësve të rreshtit të tretë (1: Po, 0: Jo)
30) Apple_car_play: Një vlerë binare që tregon praninë e integrimit Apple CarPlay / Android Auto (1: Po, 0: Jo)
31) Bluetooth: Një vlerë binare që tregon praninë e lidhjes Bluetooth (1: Po, 0: Jo)
32) Usb_port: Një vlerë binare që tregon praninë e portave USB (1: Po, 0: Jo)
33) Heated_Seats: A ka sedilje me ngrohje në makinë? (1: Po, 0: Jo)
34) Interior_color: Ngjyra e brendshme e makinës
35) Exterior_color: Ngjyra e jashtme e makinës
36) Price: Çmimi

# Atributet e datasetit

***Attributet kategorike:***  

**Nominal:**  
Brand  
Model  
Engine  
Transmission  
Fuel type  
Drivetrain  
Interior_color  
Exterior_color  

**Ordinal:**  
Damaged  
First_owner  
Personal_use  
Turbo  
Alloy_wheels  
Adaptive_cruise  
Navigation_system  
Power_liftgate  
Backup_camera  
Keyless_start  
Remote_start  
Sunroof  
Automatic_emergency_braking  
Stability_control  
Leather_seats  
Memory_seats  
Third_row_seating  
Apple_car_play  
Bluetooth  
Usb_port  
Heated_Seats  
 

***Atributet numerike:***  

**Interval:**  
Year  
Mileage  
Engine_size  
Min_mpg  
Max_mpg  

**Ratio:**  
Price  

# Tipet e të dhënave  
```
print(dataset.dtypes)
```
![data types](https://github.com/guximselmani/ML/assets/44524736/050afeae-cc08-485a-b6c3-804faeb60d82)

  

**Vlerat null**  

brand:                            3  vlera null  
model:                            3  vlera null  
year:                              3  vlera null  
mileage:                           3  vlera null  
engine:                            54  vlera null  
engine_size:                     1534  vlera null  
transmission:                     123  vlera null  
automatic_transmission:             3  vlera null  
fuel_type:                          3  vlera null  
drivetrain:                         3  vlera null  
min_mpg:                         3752  vlera null  
max_mpg:                         3752  vlera null  
damaged:                          224  vlera null  
first_owner:                      395  vlera null  
personal_using:                   246  vlera null  
turbo:                              3  vlera null  
alloy_wheels:                       3  vlera null  
adaptive_cruise_control:            3  vlera null  
navigation_system:                  3  vlera null  
power_liftgate:                     3  vlera null  
backup_camera:                      3  vlera null  
keyless_start:                      3  vlera null  
remote_start:                       3  vlera null  
sunroof/moonroof:                   3  vlera null  
automatic_emergency_braking:        3  vlera null  
stability_control:                  3  vlera null  
leather_seats:                      3  vlera null  
memory_seat:                        3  vlera null  
third_row_seating:                  3  vlera null  
apple_car_play/android_auto:        3  vlera null  
bluetooth:                          3  vlera null  
usb_port:                           3  vlera null  
heated_seats:                       3  vlera null  
interior_color:                  1478  vlera null  
exterior_color:                   270  vlera null  
price:                              3  vlera null  

<img width="323" alt="Screenshot 2024-03-19 at 22 32 12" src="https://github.com/guximselmani/ML/assets/44524736/8b1f74cb-d2f3-494a-aafc-5db88e892a24">

# Kualiteti i të dhënave  

*Në përpjekjen për të siguruar cilësinë më të lartë të të dhënave, është kryer një ekzaminim i gjerë i të dhënave. Më poshtë janë gjetjet kryesore dhe metodologjitë e aplikuara në secilin aspekt të vlerësimit të cilësisë së të dhënave.*  

duke aplikuar metoden print(dataset(dtypes)) shihen tipet e disa kolonave te cilat janë gabim në dataset
```
Kolona 'price' : object  
Kolona 'year' : float  
Kolona 'first_owner' : float  
Kolona 'personal_using' : float  
Kolona 'alloy_wheels' : float
Kolona 'adaptive_cruise_control' : float  
Kolona 'navigation_system' : float  
Kolona 'power_liftgate' : float  
Kolona 'backup_camera' : float  
Kolona 'keyless_start' : float  
Kolona 'remote_start' : float  
Kolona 'sunroof/moonroof'' : float  
Kolona 'automatic_emergency_braking' : object  
Kolona 'stability_control' : object  
Kolona 'leather_seats' : object  
Kolona 'memory_seat' : object  
Kolona 'apple_car_play/android_auto'' : object  
Kolona 'bluetooth' : float  
Kolona 'usb_port' : float  
Kolona 'heated_seats' : float  
Kolona 'automatic_transmission' : float  
```

Këto janë trajtuar me aplikimin e këtyre metodave:  
```
dataset['price'] = pd.to_numeric(dataset['price'], errors='coerce')  
dataset['year'] = dataset['year'].astype(int)  
dataset['mileage'] = dataset['mileage'].astype(int)  
boolean_columns = ['damaged', 'first_owner', 'personal_using', 'turbo', 'alloy_wheels',  
'adaptive_cruise_control', 'navigation_system', 'power_liftgate',   
'backup_camera', 'keyless_start', 'remote_start', 'sunroof/moonroof',   
'automatic_emergency_braking', 'stability_control', 'leather_seats',   
'memory_seat' , 'apple_car_play/android_auto',   
'bluetooth', 'usb_port', 'heated_seats','automatic_transmission']  

 dataset[boolean_columns] = dataset[boolean_columns].astype(bool)  
 ```

**Vlerat duplikate**  
0  
<img width="323" alt="Screenshot 2024-03-19 at 22 29 53" src="https://github.com/guximselmani/ML/assets/44524736/d8d41a7e-a80e-4af2-a274-40dc8534b334">

**Korelacioni mes min_mpg dhe max_mpg** 
![corr mpg_min_max](https://github.com/guximselmani/ML/assets/44524736/a4f209e4-2126-457a-bd46-72ae421b7245)



Faza I: Përgatitja e modelit


**Accuracy**


Faza II: Analiza dhe evaluimi
Faza III: Aplikimi i veglave të ML

