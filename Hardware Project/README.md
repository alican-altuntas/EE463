# EE 463 Hardware Project

## Wind Turbine Battery Charger

### Deadlines:
- Simulation Report - 3rd of December
- Presentation for Feedback Session - TBA
- Hardware Demo - 5th of January
- Final Report - 20th of January

### Project Description:

In this project you are required to design a battery charger. The input power of the charger is supplied by a small wind turbine generator. Your design should regulate the incoming power from wind turbine generator to feed the load and charge the battery. Thus, an AC to DC type power converter circuit has to be designed with required control actions because there are limitations for batteries in terms of their voltage and charge. Propose a solution which can regulate the output current while the input voltage is varied because of the changing wind speed.

![](WTG_Drawing.svg)

You are free to choose any topology such as (but not limited to):
 - Three-Phase Thyristor Rectifier
 - Three-Phase Diode Rectifier + Buck Converter

### Specs:

Specifications of the system are listed as follows:

 - **Input voltage**: 15 V<sub>line-to-line</sub> to 25 V<sub>line-to-line</sub>
 - **Battery capacity**: 100 Ah
 - **Battery nominal voltage**: 12 V
 - **Output current**: 10 A
 - **Output current ripple**: %20 of average current

### Project Steps:

- Choose your partners: Each group will consist of 3 people. You are free to choose your partners.

- Create a **public repo**: Open a public repo, which you will put all your work into. Please add [Ogün](https://github.com/OgunAltun) as a collaborator.

- Topology Selection: Discuss the advantages and disadvantages of each topology, and decide on a topology. You are required to present your selection process in the Complete Simulation Report.

- Analytical Calculations: After choosing a suitable topology for this case, you need to calculate the circuit parameters such as values of inductors and capacitors, duty cycle, firing angle, maximum voltage and current ratings of the circuit components.

- Simulations: According the your topology selection, you are going to run computer simulations, to prove the performance characteristics of your circuit. Start your simulations with simplest version. Then, it is best to simulate as detailed as possible to catch possible hardware problems (for example, how to generate control/gate signals).

- Component Selection: According to your analytical calculations and computer simulations decide on which components you are going to use. Not only choose the power components, but also decide on the control, and auxiliary components. Don't forget to plan logistics, it may take weeks to get some components. Loss -switching, conduction- calculations of the components should be done, after the component selection is completed.  With calculated thermal loss values, find the temperature of the components by assuming 25&deg;C ambient temperature. If necessary select a heatsink and do the thermal calculations again. If you use any magnetic component, you should choose a magnetic core from [Magnetics](https://www.mag-inc.com/) or any other supplier and do the necessary calculations.

- Implementation: Build a prototype as fast as possible, and keep iterating. You can try your design on breadborad (not suggested), but on the demo day your design should be implemented on a stripboard or PCB.

- Final Demo Day: In the demo day, you are expected to present your working prototypes. Your design should charge the battery at least for 5 minutes.

### Grading

- **Complete Simulation Report (15 pts):** A report that presents your design decisions, computer simulations, and component selection for the all parts of the project. Similar grading rules apply with previous projects (i.e. format, number of commits etc.)

- **Presentation for Feedback Session (15 pts):** Each team should present their topology selection and project design. They should describe how they selected critical components and their plan for design and manufacturing.

- **Demo Day (30 pts):** Each team is expected to present their prototype in the demo day. If you have a prototype, but somehow if it doesn't work on the demo day, you will get zero points from this part. However, if you don't come up with a prototype, or convince us that you put enough effort in building one, you will get zero points from the all hardware project (yes, even if you had the design report).

- **Final Report and Test Results (40 pts):** A report that presents your design decisions, computer simulations, component selection and test results. It should contain your results with the battery charging (data can be collected on the demo day, but preferably earlier). The report can contain any other useful tests (i.e. functionality of the switches, tests with R load etc).

#### Bonus Parts

There will be bonuses for some groups -not necessarily to a single group-. You can get extra points in any of the following. In order to get bonus points, your design should meet the minimum requirements.

- **Efficiency Bonus:** The project with the highest efficiency at rated current (10 A) will be awarded with this bonus.

- **Utilization Bonus:** A bonus will be awarded to design with the tightest semiconductor ratings. Total Voltage-Ampere rating of power semiconductors will be evaluated.

- **Compactness Bonus:** A bonus will be awarded to a project with the smallest volume (including all cabling, control circuitry, filters, connectors etc). The volume of the design will be calculated by finding the smallest possible rectangular prism that can contain the design.

- **Cheapest Design Bonus:** A bonus will be awarded to design with the cheapest unit price. You should find the costs of all the circuit components that your are going to use in Digikey for 1000 pieces and offer a Bill of Materials (BOM). You should also include the cost of PCB  using [PCBway](https://www.pcbway.com/) for again 1000 pieces.

- **Analog Controller Bonus:** If an analog controller is used to regulate the output current rather than a digital controller a bonus will be awarded.

- **Constant Current/Constant Voltage Control Bonus:** You will be awarded if your design is able to control the output voltage when the state of charge reaches the required value. [Check for details.](https://www.engineering.com/story/battery-management-systemspart-3-battery-charging-methods)

- **Extra Effort Bonus:** All of the additional converter merits such as synchronous switching, parallel converter operation and any other effort that you put outside this project definition will be awarded in grading, accordingly. Some useful examples: temperature protection, short circuit protection, over-voltage protection, battery type selection. 

- **PCB Bonus:** Implement your design on PCB. You can use PCB design softwares such as KiCad, Altium Designer, Proteus, Autocad Eagle, etc.

- **Karma Bonus:** This bonus will be awarded to one person who helps most to everyone during the project period. This bonus will be awarded by the results of anonymous voting in the demo day.

### Frequently Asked Questions

- Do I need to buy all the components?

No, we will provide some mostly used components, but not all of them. Please check the [available component list](https://github.com/odtu/ee463/blob/master/Hardware%20Project/components.md).

- Can I use the lab before demo day?

Yes, you will be able to use power electronics lab.

- What equipment will be available for us in the lab?

You will be able to use oscilloscope, power supply, soldering station, function generator and variacs. You can also use the Ground Lab after getting required safety training and permission.

- Can I also work at nights in the lab?

Unfortunately, due to safety regulations, you have to work only under technician supervision during working hours.


### Hints:

For all hints please have a look at the [tips document](https://github.com/odtu/ee463/blob/master/Hardware%20Project/tips.md).

Have a look at the hardware project presentation by course assistants [here](https://prezi.com/zqhrvmqz0ik5/ee463-hardware-project/).

# Past Years' Projects

### 2022 Teams

- [Power Rangers](https://github.com/yenescaliskan/DC_Motor_Drive): Mehmet Hakan Yel, Başak Koca, Yasin Enes Çalışkan
- [Get Rektified](https://github.com/bozgorgen/EE463_Term_Project): Ahmet Can Yulaf, Ahmet Furkan Gürsoy, Barış Özgörgen
- [VA-Method](https://github.com/irembayin/VA-Method): Nilsu Bora, İrem Bayın, Ahmet Bilgin
- [Volt Motors](https://github.com/Mehmet-Emre-Dogan/EE463_2022_TermProject): Ömer Şen, Mehmet Emre Doğan, Gamze Çelik
- [Group Name 5](https://github.com/ahmetcan-akuz/EE463_2022_Hardware_Project): Utku Deniz Altıok, Ahmetcan Akuz, Ekin Arda Çömez
- [Happy EE Friends](https://github.com/eminalpkoyuncu/EE463-Term-Project): Arda Kasım, Atilla Can Aydemir, Eminalp Koyuncu
- [Hard-Time Regulators](https://github.com/emir-altunkol/EE463-HardwareProject): Işık Emir Altunkol, Fatih Erden, İsmail Macit
- [Dolu Kapasitörü Ters Bağla](https://github.com/ozanakturk/Dolu-Kapasitoru-Ters-Bagla): Selin Ezgi Özcan, Ozan Aktürk, İsa Ersöz
- [MeteK](https://github.com/metehankk/MeteK-EE463_Project): Metehan Küçükler

### 2021 Teams

- [Enjin Drivers](https://github.com/kkaya674/EE463-TermProject): Zehra Güneş, Tuğçe Şevval Kaya, Kubilay Kaya
- [Son Motor Bükücüler](https://github.com/sametyakut/EE463-TERM-PROJECT): Berna Çorak, Musa Ulusoy, Muhammet Samet Yakut
- [Group 6](https://github.com/soysalper/METU-EEE-463-Term-Project): Ertuğrul Yolcu, Osman Yücel, Alper Soysal
- [Power Suppliers](https://github.com/ardakaslan/ee463-termproject): Emre Çelen, Özgür Arda Küçükaslan, Anıl Yalçınkaya
- [EMK](https://github.com/merterenkandilli/EE463-Term-Project-Group-1): Ecem Karamercan, Mert Eren Kandilli, Goktug Tonay
- [APPE](https://github.com/emrecakmakyurdu/EE463-Static-Power-Conversion-1--Term-Project): Zeynep Çöklü, Emre Çakmakyurdu, Uğur Cem Erdem
- [Judicator Inc](https://github.com/eiremy/EE463-Hardware-Project-G3): Ece İrem Yazır, Kaan Tütek, Hüsnü Oğuz Yorgancılar

### 2021 Videos

- [Enjin Drivers](https://www.youtube.com/watch?v=VgHXCVj92XA)
- [Son Motor Bükücüler](https://www.youtube.com/watch?v=riTFOC36qkQ)
- [Power Suppliers](https://www.youtube.com/watch?v=OlnQG5R32ZY)
- [APPE](https://www.youtube.com/watch?v=wvtaae2TDvc)

### 2020 Teams

- [Kardeşler Elektronik A.Ş](https://github.com/EnesCanbolat/EE463-Project): Enes Canbolat, Emin Un,  Berkay Uzun
- [Power Quality](https://github.com/alpercak/EE463_TermProject.git): Mustafa Mert SARIKAYA, Alper ÇAKIROĞLU, Fatih Serdar SAĞLAM
- [Power Guide](https://github.com/busranurkocak/EE463-Term-Project): Eren ÖZKARA, Yunus ÇAY, Büşranur KOÇAK
- [Distanced Power Solutions Inc.](https://github.com/ceyhunkocc/EE463-TermProject.git): Ceyhun KOÇ, Defnenur KORKMAZ, Görkem GÜLLETUTAN
- [Unlimited Power!](https://github.com/onuroztas1/EE463_Project_Onur_Halis_Halid.git): Ahmet Halis Sabırlı, Halid Filiz, Onur Öztaş, Emre Karabakla
- [Deadly Viper Assassination Squad Inc.](https://github.com/mehmetkl/EE463-Term-Project.git): Mustafa Yıldız, Ali Belli, Mehmet Kılıç

### 2020 Videos

- [Kardeşler Elektronik A.Ş](https://www.youtube.com/watch?v=OPD5CQ3YGrg&feature=youtu.be) (Best Video Bonus Winner)
- [Power Guide](https://www.youtube.com/watch?v=6BUnYYQThP8&feature=youtu.be) (Best Video Bonus Winner)
- [Distanced Power Solutions Inc.](https://www.youtube.com/watch?v=rCTESrjsp6w&ab_channel=CeyhunKo%C3%A7) (Best Video Bonus Winner)
- [Unlimited Power!](https://www.youtube.com/watch?v=Rinxe8KxoEA&feature=youtu.be) (Best Video Bonus Winner)
- [Deadly Viper Assassination Squad Inc.](https://www.youtube.com/watch?v=vXrl2gbuGQM) (Best Video Bonus Winner)

### 2019 Teams

- [Three Pole Machine](https://github.com/edsenel/ThreePoleMachine): Ogün Altun, Emre Deniz Şenel,  Fahri Türedi
- [Blue Smoke](https://github.com/pdb5627/ee463-hardware-project): Paul BROWN, İbrahim DURU, Mustafa ŞAHİN
- [3 Phases 1 Company](https://github.com/m-zeybek/3P1C_Hardware_Project): Orhun Taşoğlu, Kutay Delibaş, Mert Zeybek
- [M.P.W.U electronics](https://github.com/MERTAYDIN46/EE463_HardwareProject-M.P.W.U-electronics-): Burak kemal KARA, Cem DUMAN, Mert Yaşar AYDIN
- [N.A.M.-I Power](https://github.com/sammalek0/EE463-HardwareProject-N.A.M-I-Power): Nevzat S. Şenyayla, Muhammed Barış, Sam Ghassemi
- [Kara Şimşekler](https://github.com/nurettincavus/463karasimsekler): Deniz Boran KARACA, Nurettin ÇAVUŞ
- [Ostim Rectifiers](https://github.com/CemilUrgup/EE463-Hardware-Project-Ostim-Rectifiers): Habibullah Koçoğlu, Cemal Öztürk, Cemil Ürgüp
- [Ree-Wired](https://github.com/buryalcin/ReeWired): Beyhan Türkyılmaz, Mehmet Gürtekin, Burak Yalçın
- [Dynamic Power](https://github.com/musayeli/463-HARDWARE-Project): Hamza SOLAK, Musa YELİ, Canberk DUMAN

### 2019 Videos

- [Three Pole Machine](https://www.youtube.com/watch?v=YZUBasKc0Og)
- [3 Phases 1 Company](https://www.youtube.com/watch?v=jqYrZNpZuFA)
- [M.P.W.U electronics](https://www.youtube.com/watch?v=vqz0xIiDz8E)
- [N.A.M.-I Power](https://www.youtube.com/watch?v=fzA787_wp4Y) (Best Video Bonus Winner)
- [Kara Şimşekler](https://drive.google.com/file/d/1u6mGx2txVA8GeNq95FOMn25f3ItVCYUt/view)
- [Ostim Rectifiers](https://www.youtube.com/watch?v=GmYoqUheJWo)
- [Ree-Wired](https://www.youtube.com/watch?v=QtswupaRqzg)
- [Dynamic Power](https://www.youtube.com/watch?v=q_Ks-do5HX4)

### 2018 Teams

- [SPARK Industries](https://github.com/hhintoglu/EE463_Hardware_Project):  Huzeyfe Hintoglu, Sadık Akyar, Muhammed Hakan Karakaya
- [FosFos AG](https://github.com/sametyildirima/FosFos-AG):  Samet Yıldırım, Ozan Can İyier, Furkan Karacabey
- [BiB Power]( https://github.com/ismail-ataseven/BiB-Power): İsmail Ataseven, Berkay Sağlam, Batuhan Bülbül
- [Firing Angels](https://github.com/nailtosun/EE-463-Hardware-Project): Nail Tosun, Ali Aydın, Özgür Ertürk
- [The Third Harmonics](https://github.com/EnesAyaz/EE463-HardwareProject):Furkan Tokgöz, Enes Ayaz, Yasin Durmaz
- [The Mega Hurts](https://github.com/bulbulbahar/EE463_HardwareProject): Bahar Bülbül, Etki Açılan, Hakkı Gülcü
- [K.A.R.P.U.Z.](https://github.com/gurkandyilmaz/EE463-Hardware_Project): Ali Aydın Yamandağ, Gürkan Durmuş Yılmaz, Sonay Ulukaya
- [Freewheeling Co.](https://github.com/anilcanbudak/EE463-Hardware-Project): Anılcan Budak, Cem Akıncı, Murat Çolakoğlu
- [A.N.](https://github.com/nazliogluahmet/EE_463_proje_AN): Ahmet Nazlıoğlu
- [Smart Grid](https://github.com/ivenguzel/EE463-Harware_Project): Saliha İven Güzel, Ekin Su Saçın, Onur Külahlıoğlu
- [METU LELS](https://github.com/yusufselimkaratas/463HardwareProject): Mehmet Elen, Mert Elmas, Yusuf Selim Karataş
- [M.A.N.Power](https://github.com/nevzatsafasenyayla/M.A.N.Power): Nevzat S. Şenyayla, Akın Şavklı, Metehan Kara

### 2017 Teams

- [Kesla Motors: Melisa, Hande, Özgür](https://github.com/ghandeb/KESLA-Motors)
- [FNAG: Hakan S, Ceren, Yusuf](https://github.com/hakansrc/EE463-Hardware-Project)
- [Ripple Warriors: Eralp, Mahmut Enes](https://github.com/MehmetEralpKose/Ripple-Warriors-Hardware-Project-)
- [EMAchines: Ümit Mert, Ekin, Asım](https://github.com/UmitMertCaglar/EE463-Hardware-Project)
- [THD Defenders: Caner, Uğur, Tuna](https://github.com/caneryagci/EE_463-Hardware-Project)
- [Dank Drivers: Mert, Hakan Polat](https://github.com/hakanpolat/EE463--Dank-Drivers)
- [Ankara Instruments: Emin, Özgür, Talgat](https://github.com/emincinalioglu/Ankara-Instruments)
- [Shark Attack: Celal, Abdurrahman, Tugay](https://github.com/celalkavlak/EE463_Hardware_Project)
- [Converting Falcons: Cem, Ayberk Kaan, Olgun](https://github.com/OlgunErdogan/Converting_Falcons)
- [Raşit](https://github.com/rasitgokmen/EE463-Project)

### 2017 Videos:

- [Kesla Motors](https://www.youtube.com/watch?v=I-ww9eQDfaU)
- [FNAG](https://youtu.be/eVu52fjexhE)
- [Ripple Warriors](https://drive.google.com/file/d/1-aCfB_sSwF4t1ENeGZwWkp-CMlNDKGck/view)
- [EMAchines](https://www.youtube.com/watch?v=PyMzq8Eca7o)
- [THD Defenders](https://www.youtube.com/watch?v=gRVRT1USEpw)
- [Dank Drivers](​https://youtu.be/Q4zAWDH7_88)
- [Ankara Instruments](https://drive.google.com/open?id=17f6EGrr7mS8Uh7WiCu8BmIiLnXTHfP1c)
- [Shark Attack](​https://drive.google.com/open?id=1OIxgk-Lcdn7AT_PH-EiCHYb63u0lPHV_)
- [Converting Falcons](https://www.youtube.com/watch?v=T0_olXNja7c&feature=youtu.be)
- [Raşit](https://www.youtube.com/watch?v=tHf7YZv6PTA)

