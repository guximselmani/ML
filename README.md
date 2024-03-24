
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
*Trajtimi i tipeve do të përshkruhet më detajisht në vijim.*  
```
print(dataset.dtypes)
```
![data types](https://github.com/guximselmani/ML/assets/44524736/050afeae-cc08-485a-b6c3-804faeb60d82)

   
# Rreshtat duplikat  
**Verifikimi i rreshtave duplikat:** 
Duke përdorur këtë funksion, kemi ardh në përfundim se nuk kemi vlera duplikate
```
dataset.duplicated().sum()
```

<img width="323" alt="Screenshot 2024-03-19 at 22 29 53" src="https://github.com/guximselmani/ML/assets/44524736/d8d41a7e-a80e-4af2-a274-40dc8534b334">  

# Kolonat që nuk do të përdoren
*Per shkak të mos ndikimit në qëllimin e parashikimit do të largojmë këtë kolonë:*
third_row_seating 
```
dataset.drop(columns=['third_row_seating'], inplace=True)
```

*Per shkak që ka informata duplikate në dy kolona të ndryshme, do të largojmë këtë kolonë:*
engine  
```
dataset.drop(columns=['engine'], inplace=True)
```

*Per shkak qe per ne informate e vlefshme është ajo se a është vetura automatike apo manuale, e mbajmë vetëm kolonën automatic_transmission, do të largojmë kolonën:*
transmission  
```
dataset.drop(columns=['transmission'], inplace=True)
```

# Kualiteti i të dhënave 
```
print(dataset.isnull().sum(axis=0))
```

**Vlerat null** 
*Trajtimi i këtyre vlerave do të përshkruhet më detajisht në vijim.*
 
<img width="323" alt="Screenshot 2024-03-19 at 22 32 12" src="https://github.com/guximselmani/ML/assets/44524736/8b1f74cb-d2f3-494a-aafc-5db88e892a24">

**Pastrimi i të dhënave**
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
**Duke aplikuar këtë metodë 
```
nunique()
```
, është pa që atributet *interior_color* dhe *exterior_color* kanë shumë vlera unike
```
unique_interior_colors = dataset['interior_color'].nunique()
unique_exterior_colors = dataset['exterior_color'].nunique()

print("Number of unique interior colors:", unique_interior_colors)
print("Number of unique exterior colors:", unique_exterior_colors)
```  
![Bildschirmfoto 2024-03-24 um 17 33 20](https://github.com/guximselmani/ML/assets/44524736/a8983fd1-7626-4ce6-b3e2-e6d71dbf189f)


**Duke aplikuar këtë metodë**     
```
value_counts()
```
, është pa që sa herë përseritet ngjyra e njejtë në atributet *interior_color* dhe *exterior_color*, 
```
interior_color_counts = dataset['interior_color'].value_counts()
exterior_color_counts = dataset['exterior_color'].value_counts()
```

Prandaj duke parë shumë ngjyra tek cilat janë vetëm një herë në këtë dataset, kemi kriju një vlerë 'Other' për vlerat e ngjyrave që janë prezente në më pak se 100 vetura në komplet datasetin.

```
less_frequent_colors_exterior = exterior_color_counts[exterior_color_counts < 100].index
```
```
less_frequent_colors_exterior = interior_color_counts[interior_color_counts < 100].index
```

```
dataset['interior_color'] = dataset['interior_color'].replace(less_frequent_colors_interior, 'Other')
dataset['exterior_color'] = dataset['exterior_color'].replace(less_frequent_colors_exterior, 'Other')
```

**Në kuader të trajtimit të vlerave të zbrazëta, për shkak te numrit të vogël të rreshtave, bejmë largimin e tyre:**
 
```
dataset = dataset.dropna(subset=['price'])
dataset = dataset.dropna(subset=['exterior_color'])
dataset = dataset.dropna(subset=['interior_color'])
dataset = dataset.dropna(subset=['engine_size'])
```

Pastaj nëse aplikojme përseri funksionin 
```
print(dataset.isnull().sum(axis=0))
```
![Bildschirmfoto 2024-03-24 um 17 40 15](https://github.com/guximselmani/ML/assets/44524736/d0a9c422-03d5-4358-8929-d39f243176df)

shohim që këto dy kolona *min_mpg* edhe *max_mpg* kanë 3118 vlera të zbrazëta.

Nëse e formojmë një matricë të korrelacionit për këto dy kolona
```
columns_of_interest = ['min_mpg', 'max_mpg']
selected_data = dataset[columns_of_interest]
correlation_matrix = selected_data.corr()
print(correlation_matrix)
```
![corr mpg_min_max](https://github.com/guximselmani/ML/assets/44524736/a4f209e4-2126-457a-bd46-72ae421b7245)

Duke e parë që këto dy kolona kanë një lidhje të madhe mes vete, dhe poashtu duke e ditë qe në mënyre indirekte që vlerat për këto dy kolona derivohen nga madhësia e motorit të veturës, i largojmë keto dy kolona

```
dataset.drop(['min_mpg', 'max_mpg' ], axis=1, inplace=True)
 
```

Faza I: Përgatitja e modelit


**Accuracy**


Faza II: Analiza dhe evaluimi
Faza III: Aplikimi i veglave të ML

