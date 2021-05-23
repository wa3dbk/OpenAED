# OpenAED

A collection of manually annotated audio files for acoustic event detection (AED). 

The annotations are based on the  __[AudioSet ontology](https://research.google.com/audioset/ontology/index.html)__ (10-second segments from YouTube).


## Supported classes 
For the time being, these are the supported acoustic events : 
- :dog2: Bark (80 files)
- :bird: Bird (289 files)
- :clap: Clapping (102 files)
- :bomb: Explosion (259 files)
- :gun: Gunshot (300 files)
- :train2: Train horn (266 files)


## Annotation format 

### Filenames 
Annotation files are named after their corresponding YouTube videos : 

*- Format :*
<youtube_id>\_<start-time>\_<end-time>.txt

*- Example :*
k1swpimPFxY_30000_40000.txt

Corresponds to second 30 to second 40 in the video youtu.be/k1swpimPFxY


### Annotation files format
The annotation files follow this format :
 
<start-time> <end-time> <acoustic-event>

*- Example :*
```
>$ head -3 data/annotation/Bark/0gkLHfHJSnI_80000_90000.txt 

0.490323 2.012903 speech
1.754839 2.012903 bark
2.012903 2.877419 speech
```

### Todo : 

- [ ] Annotate more data. 
- [ ] Add more classes. 
- [ ] Develop an AED system. 
