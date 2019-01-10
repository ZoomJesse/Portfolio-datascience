# Portfolio Jesse van Noordt 1505670 
Dit is het portfolio voor KB-74 Applied data science:
2018-2019
Project group Aphasia.

**Dreamteam:**
* Erik van der Caaij,(15059421)
* Koray Poyraz,      (15068145)
* Rene Uhliar,       (14036738)

## Courses 
Voor de Minor werden online courses gegeven, Hieronder zijn de voltooide courses te vinden.
> Datacamp Screenshot:![datacamp](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Datacamp.png)
> Coursera Screenshot:![coursera](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/15.PNG) ![coursera2](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/6.PNG)

## Domain Knowledge (Literature, jargon, evaluation, existing data sets, ...)
Het domein waarin het project zich bevind is de zorgkant. Het project richt zich specifiek op aphasia patienten met een licht spraak probleem. Hierin Hebben we tijdens het project te maken met medische jargon maar ook met specifieke kenmerken en begrippen die gebruikt worden warneer er met geluid wordt gewerkt.  In de onderstaande jargon zijn de verschillende begripen beschreven. 

### Jargon:

* **ASR**: Assigned speech revocation. Ook wel spraak herkenning genoemd, vallen methodes en technieken onder die worden ontwikkeld om door computers gesproken worden te laten herkennen en verwerken. 

* **Aphasia**: Is een taalstoornis die zich betrekt over meerdere gebieden zoals spreken, taalbegrip lezen en schrijven en begrijpen. Afasie is vertaalt ook niet(a) spreken(fasie).

* **Phoneme**: Een phoneme/foneem is een verzameling van klanken die allemaal de zelfde betekenis hebben. hierbij kan gedacht worden aan bijvoorbeeld de klank "oe" van moer.

* **Diphones**: Een diphone of difoon is een spraakklank die bestaat uit twee opeenvolgende phonemes/fonen. hierbij ligt de nadruk tussen de overgang van de ene naar de andere foneem. een diphone begint vaak op de helft van de eerste phoneme en eindigt bij na de eerste helft van de eerst.

* **Seq 2 Seq**:Sequence to sequence learning is een probleem aanpak waarin een model wordt getraind op twee verschillende sequences bijvoorbeeld audio en een tekst sequence. Hierbij probeert het model aan de hand van een sequence te andere sequence te voorspellen


### Literature 

In het domein van ASR en Aphasia onderzoek in de voor van datascience zijn de volgende artikelen handig om in te kijken. 
Onderzoek van Roelant Ossewaarde, Hierbij wordt gebruik gemaakt van audio van aphasia patienten en technieken binnen datasciece om pauzes te detecteren. Ook heeft hij een artikel geschreven over computer technieken gebruikt kunnen worden bij geluid van aphasia patienten.
* [Computerized assessment of the acoustics of primary progressive aphasia](http://hdl.handle.net/11370/5ec79acc-5161-4c5d-8e09-98dc15042f4e)
* [Automated detection of unfilled pauses in speech of healthy and brain-damaged individuals](http://hdl.handle.net/11370/5ec79acc-5161-4c5d-8e09-98dc15042f4e)

Andere artiekelen die belangrijk zijn in het domein waarin het project zich bevind zijn:

* [Feature Extraction Methods LPC, PLPand MFCC In Speech Recognition](https://pdfs.semanticscholar.org/0b44/265790c6008622c0c3de2aa1aea3ca2e7762.pdf)
* [Speech Processing for Machine Learning: Filter banks, Mel-Frequency Cepstral Coefficients (MFCCs) and What's In-Between](https://haythamfayek.com/2016/04/21/speech-processing-for-machine-learning.html)

In deze artikkelen wordt de nadruk gelecht over feature extractie uit audio/spraak. dit is belangrijk voor het project en het domein om dat dit de achterliggende technieken zijn die worden gebruikt om informatie uit de audio te halen. 


## Predictive Models
De predictive model die ik heb gemaakt is een multylayer perceptron. Ik heb hierbij gemaakt van Keras dat runned op een tensorflow backend. 

Voor de Hyperparameters van het model kiezen heb ik gebruik gemaakt van de diagnostics later in het portofolio besproken. 
* Learningrate:0.003
* Dropout:0.4
* Hiddenlayers:3 hidden layers

Afbeelding van hoe hyperparameters zijn geimplementeerd:
![AFBEELDINGMODEL](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/model.PNG)

Nodebooks MLP verschillende datasets:
* [MLP_keras](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/MLP%20keras.ipynb)
* [MLP_Keras_nieuws](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/MLP%20keras-Nieuws.ipynb)

## Data collection
The data collection in dit project is gebeurt overschillende manieren. 
Door te kijken welke datasets de benodigde audio en daarbijhoorende tekst bevatten, en hiervan de kwaliteit te controleren.

### Found datasets
Naam dataset | Eigenaar |Verwijzingen
------------ |----------|-------------
CGN_2.0.3 | Nederlandse Taalunie|[link](http://lands.let.ru.nl/cgn/)
MPI diphones database|MPI|[link](https://www.mpi.nl/world/dcsp/diphones/index.html)  
Voxforge database|VoxForge|[link](http://www.voxforge.org/)
Dutch Wikipedia corpus|Rachael Tatman|[link](https://www.kaggle.com/rtatman/spoken-wikipedia-corpus-dutch)

Ook het zelf genereren van test_data voor korte experimenten door bijvoorbeeld het zelf inspreken van audio, en daar dan de bijhorende tekst van hebben.


## Data preparation

Tijdens het project heb ik mij bezig gehouden met data preparatie. Hierin is de datapreparatie gedaan in de vorm van tekst opschonings technieken. Hierbij heb ik meerdere scripts gemaakt die te tekst opschonen van lege ruimtes,lostaande woorden. In de onderstaande nodebooks is de code voor het verwijdere van lege ruimtes en witte regels:
* [Cleaning_empty_spaces](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Cleaning_empty_spaces.ipynb)

Notebook voor het verwijderen van enkele woorden:
* [Removing_solowords](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Removing_solo_words.ipynb)

Een andere vorm van data preperatie waar ik aan heb gewerk is het herformateren van de text bestanden, locatie van bestanden en de structuur in de tekst. Zo heb ik scripts geschreven voor het omzetten van alle tekstfiles naar een dicationary. 

* [Text_files_to_Dict](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Text_Files_To_Dict.ipynb)

Het splitten van zinnen in apparte regels:
* [Text_splitter](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Text_Splitter_Final.ipynb)

Het verplaatsen van files op de server zodat er gemakkelijk mee gewerkt kon worden: 
* [File_mover_onserver](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/File_Mover_Onserver.ipynb)

## Data Visualization
Bij het inladen van de dataset die gegenereerd wordt om phonime boundarys de voorspellen heb ik gekeken naar hoe de verhouding tussen de Positive voorbeelden en negative voorbeelden is.
![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Skewerd_data.PNG)
Door gebruik te maken van een methode die koray heeft ontwikkeld kunnen we de verhouding van de voorbeelden gelijk te maken. Dit voorkomt dat de classifier alleen maar 0 gaat voorspellen omdat deze voorbeelden dan veel meer voorkomen. 
![Afbeeldingerna](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Skewer_data_after.PNG)

Colorlabeling dataset
Using check 1 and 0

## Evaluation
Bij de evaluatie van de kwaliteit van de data en mijn modellen heb ik gebruikt gemaakt van verschillende maat staffen.

* Accuracy score
* N-Fold crossvalidatie:
om er voor te zorgen dat de dataset die ik gebruik goed was heb ik de mogelijkheid voor een crossvalidatie check in mijn code geimplementeerd. Hierdoor kan ik kijken dat het deel wat ik voor de training set gebruik niet specifiek goed werkt op de bij horende test set.
![afbeelding code N-fold](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/nfold.PNG)

* Handmatige sellectie   (dutchwikipedia data, controle testdata)
* ![afbeelding handmatige selectie.](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Schema%20checking%20data.PNG) 

## Diagnostics of the learning process
Tijdens het leren van moddelen heb ik gebruik gemaakt van verschillende methodes om te kijken of het leerprocess goed verloopt. Tijdens het trainen zelf heb ik ingeschakkeld dat per epochs gezien kan worden van de score in accuracy is op de training en test set, ook de loss van het model is weer te geven. 

![Afbeelding loss](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Epochs.PNG)

Door dit in de gaten te houden bij het trainen kon ik gemakelijker bepalen of de gekozen learningrate en batchsize goed was voor het huidige model. En indien nodig het eerder veranderen naar groter of klein indien de resultaten verminderende. Na het trainen van het helemodel heb ik de per epoch weergegeven wat de score was zodat ik hierin kon bepalen of mischien mijn model overfit of underfit was. ook kon ik hier goed zien of mischien minder epochs ook goed was voor het trainen van mijn model

Acucuracy | loss
--------- | ----
![Afbeelding_acuracy](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/acurracy.PNG)|![Afbeelding_kosten](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Model%20loss.PNG)

## Communication (presentations, summaries, paper, ...)
Gemaakte en gegeven presentaties 

### Gemaakte presentaties:

1. [Presentatie week 1](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%201.pptx)
2. [Presentatie week 2](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%202.pptx)
3. [Presentatie week 4](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%204.pptx)
4. [Presentatie week 5](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%205.pptx)
5. [Presentatie week 6](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%206.pptx)
7. [Presentatie week 8](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%208.pptx)
8. [Presentatie week 10](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%2010.pptx)
9. [Presentatie week 11](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Aphasia%20presentatie%20week%2011.pptx)

Paper

## List the tickets from the Scrum backlog that you worked on, linked to deliverables, own experiments, etc.
Scrum tickets for made Nodebooks and products

Product | Scrumwise Image|link|
--------- | ----|----
Research,intervieuw vragen, presentaties |![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/sprint%201.PNG)|[link](https://www.scrumwise.com/scrum/#/taskboard/sprint/vooronderzoek-sprint-1/id-84641-10738-13)
Datacamp,Presentatie|![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/sprint%202.PNG)|[link](https://www.scrumwise.com/scrum/#/taskboard/sprint/sprint-2/id-84641-10760-3)
TextCleaning,Tesktformating,Presentatie|![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Sprint%203.PNG)|[link](https://www.scrumwise.com/scrum/#/taskboard/sprint/sprint-3/id-84641-11141-1)
Research,Featureselection,Codering database|![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/sprint%204.PNG)|[link](https://www.scrumwise.com/scrum/#/taskboard/sprint/sprint-4/id-84641-11570-1)
Paperselection, Coursera, Codering diphones, Generation testdata|![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/sprint%205.PNG)|[link](https://www.scrumwise.com/scrum/#/taskboard/sprint/sprint-5/id-84641-11715-1)
MLP classifier, presentaties|![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/sprint%206.PNG)|[link](https://www.scrumwise.com/scrum/#/taskboard/sprint/sprint-6/id-84641-12013-3)
CorpusGesprokenNederlands uitzoeken|![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Sprint%207.PNG)|[link](https://www.scrumwise.com/scrum/#/taskboard/sprint/sprint-7/id-84641-12767-1)


## Add any other assignment you feel is evidence of your abilities
