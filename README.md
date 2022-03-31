# LU_FMOF_Moderna_Fizika_I

Šajā vietnē var atrast failus, kurus izmantosim Latvijas Universitātes Fizikas, matemātikas un optometrijas fakultātes (LU FMOF) bakalaura programmas kursa "Moderna Fizika I" praktisko darbu ietvaros. Tiek izmantota Julia valoda (https://www.julialang.org). Faili ir Jupyter (.ipynb) vai Pluto (.jl) klādes. 

Ar "Jupyter" failiem var strādāt izmantojot "Jupyter Notebook", ko var atrast, piemērram, Anaconda (https://www.anaconda.com). Ir jābūt instalēta uz datora "Julia" valoda (https://julialang.org/downloads/) kā arī Anaconda vai cita "Jupyter Notebook" istenošana.  Turklāt, visas nepieciešamas paketes ir jāinstalē "Julia" vidē ar pakešu menedžeri Pkg.jl. Pastav arī vairākas iespējas palaist Jupyter klādes mākonī.  

Lai strādātu ar Pluto klādi, ir jābūt instalētai uz datora "Julia", bet par paketēm nav jārūpējās. Vienīgi, ir jāinstalē pati "Pluto.jl" pakete. Instrukcija var atrast šeit: https://www.juliapackages.com/p/pluto. Hīpersaite uz "FAQ" ir ļoti noderīgi, piemēram sadaļa par Pluto.jl izmantošanas pamatiem: https://github.com/fonsp/Pluto.jl/wiki/%F0%9F%94%8E-Basic-Commands-in-Pluto  .  

# "Julia" Instalēšana un palaišana
1. Lejupladēsim "Current stable release" no https://julialang.org/downloads/ attiecīgajai sistēmai. Izmantosim "Installer", ja mums ir tiesības installēt programmatūra datorā, palaidām "Installer" un sekosim instrukcijas. Ja nav tādas tiesības, varam lejupielādēt "portable" versiju. To liksim kādā mapē, klikšķinām ar labo peles pogu un izvelēsim "Extract all". 
2. Ejam uz julia-x.x.x/bin mapi un spiedīsim "julia" aplikāciju. Atvērsies teksta logs un mēs varam strādāt tiklīdz paradīsies "julia >".

# Pluto.jl Instalēšana un palaišana
1. Startēsim "Julia" programmu.
2. Rakstīsim "import Pluto" un spiest <ENTER>. Visticamāk būs ziņa, ka tādas paketes nav, bet reģistrijā atrodās pakete Pluto.jl, un uzdos jautājumu vai vēlāmies to instalēt. Spiedīsim [y]. Tiek lejupieladētas un istalētas Pluto.jl pakete un visas tam nepieciešamas paketes.
3. Rakstīsim "Pluto.run()". Pēc īsa laika atvērsies "Pluto.jl" logs mūsu interneta pārlukā.

  
