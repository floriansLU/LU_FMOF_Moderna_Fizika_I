# LU_FMOF_Moderna_Fizika_I

Šajā vietnē var atrast failus, kurus izmantosim Latvijas Universitātes Fizikas, matemātikas un optometrijas fakultātes (LU FMOF) bakalaura programmas kursa "Moderna Fizika I" praktisko darbu ietvaros. Tiek izmantota "Julia" valoda (https://www.julialang.org). Faili ir Jupyter (.ipynb) vai Pluto (.jl) klādes. 

Ar "Jupyter" failiem var strādāt izmantojot "Jupyter Notebook", ko var atrast, piemērram, Anaconda (https://www.anaconda.com). Ir jābūt instalēta uz datora "Julia" valoda (https://julialang.org/downloads/) kā arī Anaconda vai cita "Jupyter Notebook" istenošana.  Turklāt, visas nepieciešamas paketes ir jāinstalē "Julia" vidē ar pakešu menedžeri Pkg.jl. Pastav arī vairākas iespējas palaist Jupyter klādes mākonī.  

Lai strādātu ar Pluto klādi, ir jābūt instalētai uz datora "Julia", bet par paketēm nav jārūpējās. Vienīgi, ir jāinstalē pati "Pluto.jl" pakete. Instrukcija var atrast [šeit](https://www.juliapackages.com/p/pluto). Hīpersaite uz "FAQ" ir ļoti noderīgi, piemēram [sadaļa](https://github.com/fonsp/Pluto.jl/wiki/%F0%9F%94%8E-Basic-Commands-in-Pluto) par "Pluto.jl" izmantošanas pamatiem.     

Te ir labs [video](https://www.youtube.com/embed/OOjKEgbt8AI), kas apraksta kā instalēt "Julia" un "Pluto.jl" un kā ar viņiem sākt darboties.


## "Julia" Instalēšana un palaišana
1. Lejupladēsim "Current stable release" no https://julialang.org/downloads/ attiecīgajai sistēmai. Izmantosim "Installer", ja mums ir tiesības installēt programmatūra datorā, palaidām "Installer" un sekosim instrukcijas. Ja nav tādas tiesības, varam lejupielādēt "portable" versiju. To liksim kādā mapē, klikšķinām ar labo peles pogu un izvelēsim "Extract all". 
2. Ejam uz julia-x.x.x/bin mapi un spiedīsim "julia" aplikāciju. Atvērsies teksta logs un mēs varam strādāt tiklīdz paradīsies "julia >". Tas izskatās šādi:

![This is an image](/assets/images/Julia-startup.PNG)

## Pluto.jl Instalēšana un palaišana
1. Palaižam "Julia" programmu.
3. Nospiežam `]`. Uzreiz būsim pakešu menedžerā. To varam zināt, jo `Julia>` pārveidosies `Pkg>`
4. Rakstām `add Pluto` un spiedīsim <ENTER>:
  
![add_Pluto](/assets/images/add_Pluto.PNG)
  
4. Nospiežam `BACKSPACE`, lai aizietu no pakešu menedžera un atgrieztos Julia. 
  
## Pluto klādes palaišana
1. No `Julia`", rakstam `Pluto.run()` un nospiežam `ENTER`:
  
![Pluto_run](/assets/images/Pluto_run.PNG)

Pēc īsa laika Pluto.jl atvērs logu mūsu interneta pārlukā.
2. Ejam uz Pluto.jl logu mūsu interneta pārlukā.
  
3. Dialoga kastītē zem "Open from file" liekam hīpersaiti uz vēlamo Pluto klādi (fails, kas beidzās ar .jl) no šīs Github vietnes. Alternatīvi, var lejupladēt šo failu uz savu datoru un atvērt no datora. 
  
4. Jāgaida nedaudz kamēr tiek instalētas nepieciešamas paketes. (Kamēr tas notiek, var iepazīties ar mācību mērķiem un saturu.)
  
5. Pēc tam, zem katras šūnas ir "Play" pogs. Spiežot šo pogu, palaidām paveles, kas atrodas tajā šūnā. Rezultāts tiks radīts virs šūnas. 
  
6. Mēs varam arī mainīt kodu katrā šūna un skatīties, kas tur notiek.
  
7. Ja negribam redzēt kodu, to varam slept vai atslēpt 👁️ pogu. 
  
8. Neaizmirsam saglabāt klādi savā datorā, it īpaši, ja esam veikuši kādas izmaiņas. To var darīt lapas augšējā daļā. Pa vidu ir dialoga kastīte "Save notebook". 
   
  ![file_dialog](/assets/images/Open_from_file.PNG)
   
  Tur rakstam faila nosaukumu ar "path" (piemēram C:\User\vārds\Documents\Pluto\manaKlade.jl, ja būsim izveidojuši iepriekš mapi C:\User\vārds\Documents\Pluto). Varam atjaunot saglabāšanu spiežot `Ctrl`-`S`. Vēl var lapas augšējā pusē pa labi spiest uz "Export" (trīsstūris un aplis) 
  
  ![export](/assets/images/export.PNG) 
  
  un eksportēt mūsu klādē 3 formātos: .jl, .html vai .pdf. 
  
## Pluto.jl aizveršāna

1. Klikšķinām uz "Pluto" logo lapas augšējā daļā pa kreisi.
  
   ![menu](/assets/images/main_menu.PNG) 
  
2. Aizveram visas atvērtas klādes, kliķšinot "x" blakus atvērtām klādēm sarakstā.
  
     ![exit](/assets/images/logging-out.PNG) 
  
3. Ejam uz "Julia logu", spiežam `Ctrl`-`C`. 
4. Aizveram visus logus. 
  
## Dažas piezīmes
1. Viena liela atšķirība starp "Pluto" klādēm un "Jupyter" klādēm ir tas, ka "Pluto" stingri kontrolē, ka mainīgie netiek nejauši pārdefinēti. Tas nozīmē, ka drīkst kādu mainīgu definēt tikai vienreiz klādē. Jāizmanto cits mainīgā nosaukums, ja vēlāmies vairākās definīcijas. Labums ir tas, ka atšķirībā no "Jupyter", nevar notikt, ka mainīgā vērtība ir atkarīga no secības ar kuru šūnas tiek palaistas. 
2. Vēl "Pluto.jl" klāde vēlas veicināt īsas šūnas. Tas nozīmē, ka paveļu bloki, kas sastav no vairākām rindām, ir jāliek starp "begin" un "end" pavēlēm.  
