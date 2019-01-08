# Portfolio Jesse van Noordt 1505670 
Dit is het portfolio voor KB-74 Applied data science:

## Courses 
Voor de Minor werden online courses gegeven, Hieronder zijn de voltooide courses te vinden.
> Datacamp Screenshot:![datacamp](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Datacamp.png)
> Coursera Screenshot:

## Domain Knowledge (Literature, jargon, evaluation, existing data sets, ...)
* Jargon:
* ASR:
* Aphasia:
* Phoneme:
* Diphones:
* Seq 2 Seq:

### Found datasets
Naam dataset | Eigenaar |Verwijzingen
------------ |----------|-------------
CGN_2.0.3 | Nederlandse Taalunie|[link](http://lands.let.ru.nl/cgn/)
MPI diphones database|MPI|[link](https://www.mpi.nl/world/dcsp/diphones/index.html)  
Voxforge database|VoxForge|[link](https://www.kaggle.com/rtatman/spoken-wikipedia-corpus-dutch)

### Literature 
Onderzoek van Roelant Ossewaarde.
* [Computerized assessment of the acoustics of primary progressive aphasia](http://hdl.handle.net/11370/5ec79acc-5161-4c5d-8e09-98dc15042f4e)
* [Automated detection of unfilled pauses in speech of healthy and brain-damaged individuals](http://hdl.handle.net/11370/5ec79acc-5161-4c5d-8e09-98dc15042f4e)
* [Feature Extraction Methods LPC, PLP and MFCC In Speech Recognition](https://pdfs.semanticscholar.org/0b44/265790c6008622c0c3de2aa1aea3ca2e7762.pdf)
* [Speech Processing for Machine Learning: Filter banks, Mel-Frequency Cepstral Coefficients (MFCCs) and What's In-Between] (https://haythamfayek.com/2016/04/21/speech-processing-for-machine-learning.html)


Onderzoek over features die we gebruiken.

## Predictive Models
* [MLP_keras](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/MLP%20keras.ipynb)
* [File_mover_onserver](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/File_Mover_Onserver.ipynb)
* [MLP_Keras_nieuws](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/MLP%20keras-Nieuws.ipynb)
* [Text_files_to_Dict](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Text_Files_To_Dict.ipynb)




## Data preparation
* [Text_files_to_Dict](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Text_Files_To_Dict.ipynb)
* [Cleaning_empty_spaces](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Cleaning_empty_spaces.ipynb)
* [Text_splitter](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Text_Splitter_Final.ipynb)
* [Removing_solowords](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Removing_solo_words.ipynb)

Cleaning text
Reformating to used in code form koray
CGNmaken
Moving and formating data

## Data Visualization
Bij het inladen van de dataset die gegenereerd wordt om phonime boundarys de voorspellen heb ik gekeken naar hoe de verhouding tussen de Positive voorbeelden en negative voorbeelden is.
![Afbeelding](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Skewerd_data.PNG)
Door gebruik te maken van een methode die koray heeft ontwikkeld kunnen we de verhouding van de voorbeelden gelijk te maken. Dit voorkomt dat de classifier alleen maar 0 gaat voorspellen omdat deze voorbeelden dan veel meer voorkomen. 
![Afbeeldingerna](https://github.com/ZoomJesse/Portfolio-datascience/blob/master/Skewer_data_after.PNG)

Colorlabeling dataset
Using check 1 and 0

## Data collection
Dataset 
tabel datasets die we gevonden hebben.
Wikipedia
VoxForge
UVA


## Evaluation

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

Samenvattingen onderzoeken
Paper

## List the tickets from the Scrum backlog that you worked on, linked to deliverables, own experiments, etc.
## Add any other assignment you feel is evidence of your abilities
