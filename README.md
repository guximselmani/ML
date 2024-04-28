Faza I: Përgatitja e modelit

# Pasqyrë e pergjithshme
* Ky projekt zhvillohet si pjesë e kurrikulës në Universitetin e Prishtinës, në kuadër të studimeve të nivelit Master të Fakultetit të Inxhinierisë Elektrike dhe Kompjuterike, si aktivitet i lëndës 'Machine Learning'.
Fokusohet në aspektet thelbësore të aplikimit të algoritmeve të ML në një domen të caktuar.
  
* Profesor:  
  Prof. Dr. Lule AHMEDI

* Asistent:  
  M. Sc. Mërgim HOTI
  
* Autor:  
  Guxim Selmani

* Viti akademik:
  2023/2024
  
# Qëllimi
Objektivi kryesor i këtij projekti është të demonstrojë në përgjithësi përgatitjen, përpunimin dhe vizualizimin e të dhënave ashtu që të mund të zbatohen teknika dhe metodologji të ndryshme që lidhen me përgatitjen dhe krijimin e modelit parashikues dhe zbatimin e algoritmeve te ML.

# Hyrje
Ky dataset përmban një grup të të dhënave  për  makina të përdorura. Ai përfshin veçori të ndryshme të makinave si marka, modeli, viti, kilometrazhi, detajet e motorit, lloji i transmisionit, lloji i karburantit, çmimi, lëvizja dhe më shumë. Ai përfshin informacion mbi atributet e ndryshme të automjeteve dhe ndikimin e tyre, të cilat mund të përdoren për të marrë vendime të informuara në lidhje pronësine e automjetit. Pra qëllimi i këtij grupi të dhënash është të vlerësojë performancën e modeleve të mësimit të makinerive për të parashikuar nësë pronari i makinës, është apo nuk është pronari i parë i tij.

# Integrimi i të dhënave
Në këtë punim, integrimi i të dhënave është thelbësore për të ndërtuar një dataset të unifikuar për analizë

Ne i bashkojmë këto nën-grupe të dhënash duke përdorur librarinë Pandas, veçanërisht funksionin concat(). Duke bashkuar këto nën-grupe të dhënash, ne krijojmë një grup të dhënash të vetme,  'combined_dataset.csv'. Ky grup të dhënash shërben si bazë për analizën dhe detyrat tona të modelimit të mëvonshëm, duke na mundësuar të nxjerrim njohuri më të forta dhe të marrim vendime të informuara.

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

**Binarizimi**
boolean_columns = ['damaged', 'first_owner', 'personal_using', 'turbo', 'alloy_wheels',  
'adaptive_cruise_control', 'navigation_system', 'power_liftgate',   
'backup_camera', 'keyless_start', 'remote_start', 'sunroof/moonroof',   
'automatic_emergency_braking', 'stability_control', 'leather_seats',   
'memory_seat' , 'apple_car_play/android_auto',   
'bluetooth', 'usb_port', 'heated_seats','automatic_transmission']  

 dataset[boolean_columns] = dataset[boolean_columns].astype(bool)  
 ```
**Duke aplikuar këtë metodë**  
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

Prandaj duke parë shumë ngjyra tek cilat janë paraqit shumë rrallë në këtë dataset, kemi kriju një vlerë 'Other' për vlerat e ngjyrave që janë prezente në më pak se 100 vetura në komplet datasetin.
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

# Të dhënat e plota
Pas trajtimit dhe pastrimit të të dhënave, aplikojmë këto funksione:  
```
print(dataset.isnull().sum(axis=0))
num_rows, num_columns = dataset.shape

print("Number of columns:", num_columns)
print("Number of rows:", num_rows)
```
![Bildschirmfoto 2024-03-24 um 17 52 11](https://github.com/guximselmani/ML/assets/44524736/aba0e6ff-890a-409f-8b79-b0e1be43cebc)  

# Diskretizimi  
**Diskretizimi i kolonës 'engine_size'**  
![image](https://github.com/guximselmani/ML/assets/44524736/e8e72fbe-6b6a-4ae4-82ac-a366894eddab)  

**Diskretizimi i kolonës 'drivetrain'**  
![Bildschirmfoto 2024-03-24 um 19 36 47](https://github.com/guximselmani/ML/assets/44524736/8d06ad64-4998-4942-9d44-aba3458fb9fd)  

**Diskretizimi i kolonës 'fuel'**  
![Bildschirmfoto 2024-03-24 um 19 37 17](https://github.com/guximselmani/ML/assets/44524736/9d96ce3f-f6fc-4cae-8bba-b7f8e9e83456)  

# Transformimi
**Normalizimi i atributeve numerike**
Në rastet kur atributet numerike kanë shkallë të ndryshme duhet të  merren parasysh aplikimet e teknikave të shkallëzimit të veçorive si standardizimi ose normalizimi për t'i sjellë ato në një shkallë të ngjashme. Pasi kjo mund të ndihmojë në përmirësimin e performancës së algoritmeve të ML.

```
numerical_data = dataset[['year', 'mileage']]

min_max_scaler = MinMaxScaler()
scaled_data_minmax = min_max_scaler.fit_transform(numerical_data)
scaled_data_minmax_df = pd.DataFrame(scaled_data_minmax, columns=numerical_data.columns)
print(scaled_data_minmax_df.head())
```
![Bildschirmfoto 2024-03-24 um 20 18 56](https://github.com/guximselmani/ML/assets/44524736/b4aa1438-98f9-4ec0-9102-8189d324efe8)

# Detektimi i outliers
*Në këtë fazë, u fokusuam në identifikimin dhe menaxhimin e të dhënave outliers, korrigjimin e zbulimeve të pasakta dhe kryerjen e një eksplorimi të plotë të grupit të të dhënave, duke përfshirë përmbledhjen e statistikave dhe analizat me shumë variacione.*

**Detektimi i outlier duke përdorur IQR (Boxplots) për atributet numerike**
Duke pêrdorur IQR, për detektimin e outliers në atributet numerike kemi fituar rezultatin:
```
year: 819
mileage: 446
price: 1086
```

![Bildschirmfoto 2024-03-24 um 22 32 16](https://github.com/guximselmani/ML/assets/44524736/2d76d2b8-db75-46cd-a152-65d120b98372)
![Bildschirmfoto 2024-03-24 um 22 32 41](https://github.com/guximselmani/ML/assets/44524736/e75bb8ee-30e6-4ac9-bb95-d9ec9479fe5f)
![Bildschirmfoto 2024-03-24 um 22 33 01](https://github.com/guximselmani/ML/assets/44524736/109a45ce-b2dd-47da-8ce5-2c0f8c5031a6)

pas largimit të tyre:
```
Shape of dataset before removing outliers: (20774, 31)
Shape of dataset after removing outliers: (18571, 31)
```
![Bildschirmfoto 2024-03-24 um 22 33 36](https://github.com/guximselmani/ML/assets/44524736/b02fc55e-eaa4-4137-88b5-699d0078642b)
![Bildschirmfoto 2024-03-24 um 22 34 02](https://github.com/guximselmani/ML/assets/44524736/01a244fc-cacb-4936-9b10-81a734e3b78e)
![Bildschirmfoto 2024-03-24 um 22 34 24](https://github.com/guximselmani/ML/assets/44524736/9fdcee73-7fa6-445c-9708-62c230e085c4)




**Enkodimi i variablava kategorike**
Variablat kategorikë si interior_color, exterior_color, brand dhe model janë të enkoduara duke përdorur metodën fit_transform() të LabelEncoder. Kjo i konverton etiketat kategorike në paraqitje numerike.
 

# Selektimi i veçorive dhe variabla e targetit

X krijohet duke larguar variablin e targetit *first_owner* nga grupi i të dhënave. Kjo do të përmbajë të gjitha tiparet e përdorura për predikim.
Y i është caktuar ndryshorja e targetit *first_owner*. Kjo do të përdoret për të trajnuar modelin për të parashikuar variablin e synuar bazuar në veçoritë.

# Ndarja e të dhënave në grupe trajnimi dhe testimi
*Në përgjithësi, ky segment kodi përgatit grupin e të dhënave për trajnimin e një modeli RandomForestClassifier duke koduar variabla kategorike, duke e ndarë grupin e të dhënave në grupe trajnimi dhe testimi dhe duke zgjedhur veçoritë e duhura dhe variablin e synuar.*
```
# Select features and target variable
X = dataset.drop('first_owner', axis=1)  # Features
y = dataset['first_owner']  # Target variable

# Split the data into training and testing sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
```
Funksioni train_test_split() përdoret për të ndarë grupin e të dhënave në grupe trajnimi dhe testimi.
X_train, X_test: Këto variabla përmbajnë veçoritë për grupet e trajnimit dhe testimit.
y_train, y_test: Këto variabla përmbajnë variablen e targetuar për grupet e trajnimit dhe testimit.
test_size=0.2: Ky parametër specifikon që 20% e të dhënave do të përdoren për testim, dhe 80% e mbetur do të përdoret për trajnim.
random_state=42: Ky parametër siguron riprodhueshmëri duke vendosur një bazë për gjeneratorin e numrave të rastësishëm.


```
# Number of rows in the original dataset
total_rows = len(dataset)

# Number of rows for training
rows_training = len(X_train)

# Number of rows for testing
rows_testing = len(X_test)

print("Total rows:", total_rows)
print("Rows for training:", rows_training)
print("Rows for testing:", rows_testing)
```
![Bildschirmfoto 2024-03-24 um 22 12 13](https://github.com/guximselmani/ML/assets/44524736/140f78c9-6bd3-4422-b142-5cd133e6183c)


# Faza II: Analiza dhe evaluimi  
Gjatë trajnimit, modeli mëson paterne në të dhënat që lidhen me variablen e targetuar.
Prandaj është thelbësore të analizohet dhe krahasohet performanca e modelit kundrejt algoritmeve të tjera për të përcaktuar nëse nevojiten optimizime të mëtejshme shtesë. Do të analizohen ndarje të ndryshme të të dhënave testuese dhe trajnuese për të vlerësuar performancën duke përdorur metrikat  Accuracy, F1-score, Recall dhe Precision.

Ne do të analizojmë rezultatet e trajnimit të 4 algoritmeve të ndryshme të cilat janë:  

* Random Forest Classifier
* Logistic Regression
* SVM
* Naive Bayes

Me aplikimin e algoritmit <strong>Random Forest Classifier</strong>:  
*Rasti I*  
Raporti i të dhënave testuese dhe trainuese është 0.1 me 0.9
```
Accuracy: 0.7670837343599615
F1-score (Random Forest): 0.7744641192917054
Recall (Random Forest): 0.7832233741753063
Precision (Random Forest): 0.7658986175115208
```
*Rasti II*  
Raporti i të dhënave testuese dhe trainuese është 0.2 me 0.8
```
Accuracy: 0.770878459687124
F1-score (Random Forest): 0.7801385681293302
Recall (Random Forest): 0.7874125874125875
Precision (Random Forest): 0.7729977116704806
```
*Rasti III*  
Raporti i të dhënave testuese dhe trainuese është 0.3 me 0.7
```
Accuracy: 0.7623937108936307
F1-score (Random Forest): 0.7740655987795575
Recall (Random Forest): 0.7760783114102172
Precision (Random Forest): 0.7720632988435788
```
*Rasti IV*  
Raporti i të dhënave testuese dhe trainuese është 0.4 me 0.6
```
Accuracy: 0.7567990373044524
F1-score (Random Forest): 0.7679944897256342
Recall (Random Forest): 0.7617854702801184
Precision (Random Forest): 0.7743055555555556
```
***Bazuar në rezultatet e gjeneruara nga këto metrika, duket se Rasti II (raporti i ndarjes së të dhënave testuese dhe trajnuese prej 0,2:0,8) gjeneron rezultatet më të mira në krahasim me rastet e tjera për Random Forest Classifier.***


Me aplikimin e algoritmit <strong>Logistic Regression</strong>:  
*Rasti I*  
Raporti i të dhënave testuese dhe trainuese është 0.1 me 0.9
```
Accuracy (Logistic Regression): 0.670837343599615
F1-score (Logistic Regression): 0.6992084432717678
Recall (Logistic Regression): 0.7492931196983977
Precision (Logistic Regression): 0.6553998351195384
```
*Rasti II*  
Raporti i të dhënave testuese dhe trainuese është 0.2 me 0.8
```
Accuracy (Logistic Regression): 0.6803850782190133
F1-score (Logistic Regression): 0.7129269347168181
Recall (Logistic Regression): 0.7687645687645688
Precision (Logistic Regression): 0.6646513502619912
```
*Rasti III*  
Raporti i të dhënave testuese dhe trainuese është 0.3 me 0.7
```
Accuracy (Logistic Regression): 0.6821755174073479
F1-score (Logistic Regression): 0.7188076650106459
Recall (Logistic Regression): 0.7745487916794127
Precision (Logistic Regression): 0.6705508474576272
```
*Rasti IV*  
Raporti i të dhënave testuese dhe trainuese është 0.4 me 0.6
```
Accuracy (Logistic Regression): 0.678459687123947
F1-score (Logistic Regression): 0.7148954332052924
Recall (Logistic Regression): 0.7629241630608062
Precision (Logistic Regression): 0.672555711704477
```
***Bazuar në rezultatet e gjeneruara nga këto metrika, duket se Rasti III (raporti i ndarjes së të dhënave testuese dhe trajnuese prej 0.3:0.7) performon pak më mirë në krahasim me rastet e tjera për Regresionin Logjistik.***


Me aplikimin e algoritmit <strong>SVM</strong>  
*Rasti I*  
Raporti i të dhënave testuese dhe trainuese është 0.1 me 0.9
```
Accuracy (SVM): 0.6886429258902791
F1-score (SVM): 0.7084272194682288
Recall (SVM): 0.7408105560791706
Precision (SVM): 0.6787564766839378
```
*Rasti II*  
Raporti i të dhënave testuese dhe trainuese është 0.2 me 0.8
```
Accuracy (SVM): 0.69338146811071
F1-score (SVM): 0.7172658677319129
Recall (SVM): 0.7533799533799533
Precision (SVM): 0.6844557390936044
```
*Rasti III*  
Raporti i të dhënave testuese dhe trainuese është 0.3 me 0.7
```
Accuracy (SVM): 0.6892347184341409
F1-score (SVM): 0.7171023806046444
Recall (SVM): 0.7509941878250229
Precision (SVM): 0.6861375069871437
```
*Rasti IV*  
Raporti i të dhënave testuese dhe trainuese është 0.4 me 0.6
```
Accuracy (SVM): 0.6878459687123947
F1-score (SVM): 0.7156325367244026
Recall (SVM): 0.7433386472329765
Precision (SVM): 0.6899175649968294
```
***Bazuar në rezultatet e gjeneruara nga këto metrika, duket se Rasti II (raporti i ndarjes së të dhënave testuese dhe trajnuese prej 0.2:0.8) performon pak më mirë në krahasim me rastet e tjera për SVM.***


Me aplikimin e algoritmit <strong>Naive Bayes</strong>  
*Rasti I*  
Raporti i të dhënave testuese dhe trainuese është 0.1 me 0.9
```
Accuracy (Naive Bayes): 0.7040423484119346
F1-score (Naive Bayes): 0.7492865878516103
Recall (Naive Bayes): 0.8661639962299718
Precision (Naive Bayes): 0.6602011494252874
```
*Rasti II*  
Raporti i të dhënave testuese dhe trainuese është 0.2 me 0.8  
```
Accuracy (Naive Bayes): 0.7051744885679904
F1-score (Naive Bayes): 0.7542627883650952
Recall (Naive Bayes): 0.8764568764568764
Precision (Naive Bayes): 0.6619718309859155
```
*Rasti III*  
Raporti i të dhënave testuese dhe trainuese është 0.3 me 0.7
```
Accuracy (Naive Bayes): 0.7108936306754372
F1-score (Naive Bayes): 0.7569463177771784
Recall (Naive Bayes): 0.8583664729275008
Precision (Naive Bayes): 0.6769601930036189
```
*Rasti IV*  
Raporti i të dhënave testuese dhe trainuese është 0.4 me 0.6
```
Accuracy (Naive Bayes): 0.7086642599277978
F1-score (Naive Bayes): 0.755725961053375
Recall (Naive Bayes): 0.85288089273514
Precision (Naive Bayes): 0.6784420289855072
```
***Bazuar në rezultatet e gjeneruara nga këto metrika, duket se Rasti III (raporti i ndarjes së të dhënave testuese dhe trajnuese prej 0.3:0.7) performon pak më mirë në krahasim me rastet e tjera për Naive Bayes.***

Në këtë analizë, janë përdorur katër algoritme të ndryshme për të modeluar dhe parashikuar të dhënat. Për secilin algoritem, janë raportuar rezultatet e performancës për katër raste të ndryshme, ku ndarja e të dhënave testuese dhe trajnuese është ndryshuar për secilin rast.

*Random Forest Classifier:*    
Rezultatet më të mira për këtë algoritem janë vërejtur në rastin e dytë, ku raporti i ndarjes së të dhënave është 0.2 me 0.8.  
*Logistic Regression:*   
Performanca më e mirë është evidentuar në rastin e tretë,  ku raporti i ndarjes së të dhënave është 0.3:0.7.  
*SVM:*    
Rezultatet më të mira për SVM janë vërejtur gjithashtu në rastin e dytë,  ku raporti i ndarjes së të dhënave është 0.2:0.8.  
*Naive Bayes:*       
Performanca më e mirë është vlerësuar në rastin e tretë,  ku raporti i ndarjes së të dhënave është 0.3:0.7.  

Këto rezultate vërtetojnë se ndryshimi i ndarjes së të dhënave testuese dhe trajnuese mund të ketë ndikim në performancën e algoritmeve të mësipërm.  Në rastin tonë saktësi më të madhe ka gjeneruar algoritmi Random Forest Classifier
Një reprezentim më të mirë të këtyre rezultateve të gjeneruara, mund të i paraqesim përmes visualizimit si më poshtë:  
# Vizualizimi i performancën së secilit algoritëm në metrikat përkatëse.
<img width="715" alt="Bildschirmfoto 2024-04-27 um 00 12 28" src="https://github.com/guximselmani/ML/assets/44524736/92c6c70d-3c50-4d46-a4e1-bb254a94c5cc">

<img width="715" alt="Bildschirmfoto 2024-04-27 um 00 12 44" src="https://github.com/guximselmani/ML/assets/44524736/33916c5c-9bfc-4658-a262-d5cced4cb38a">

Faza III: Aplikimi i veglave të ML
# Pse algoritmi Random Forest Classifier?
*Random Forest* është një algoritëm që mund përdorët për detyra klasifikimi si në rastin tonë nëse është pronari i parë apo jo,
avantazheve që ofron ky algoritem:

*Saktësia e lartë:* Random Forest tenton të sigurojë saktësi të lartë në krahasim me shumë algoritme të tjera. Funksionon mirë si me veçoritë numerike ashtu edhe me ato kategorike dhe mund të trajtojë një numër të madh të variablave hyrëse pa u përshtatur shumë.


*E qëndrueshme ndaj Overfitting:* Random Forest është më pak i prirur ndaj mbi përshtatjes në krahasim me decision trees. Duke trajnuar shumë pemë në nëngrupe të ndryshme të të dhënave dhe duke mesatarizuar parashikimet e tyre, zvogëlon rrezikun e përshtatjes së tepërt ndaj zhurmës në të dhënat e trajnimit.

*Trajton marrëdhëniet jo-lineare:* Random Forest mund të kapë marrëdhënie komplekse jolineare midis veçorive dhe targetit së synuar. Ai e bën këtë duke marrë parasysh kufijtë e shumëfishtë të vendimeve të krijuara nga pemë të ndryshme, duke e lejuar atë të modelojë modele të ndërlikuara në të dhëna.

*Trajton vlerat që mungojnë*: Random Forest mund të trajtojë vlerat që mungojnë në grupin e të dhënave. Ai e arrin këtë duke mesatarizuar parashikimet nga shumë pemë, ku çdo pemë mund të trajtojë vlerat që mungojnë në mënyrë të pavarur gjatë trajnimit dhe parashikimit.

*Rëndësia e veçorive:* Random Forest ofron një masë të rëndësisë së veçorive, e cila tregon kontributin e çdo veçori në performancën parashikuese të modelit. Ky informacion mund të jetë i dobishëm për zgjedhjen e veçorive dhe për të kuptuar marrëdhëniet themelore në të dhëna.


 
 

