---
layout: post
title: "eNATL60 model simulations in preparation for SWOT altimeter mission."
date: 2019-05-12
---


In collaboration with the [Ocean Next](http://ocean-next.fr) crew, **our group has just completed a new North Atlantic simulations campaign** in preparation for the upcoming SWOT altimeter mission (to be launched in 2021). 
The SWOT altimeter mission will provide measurements of sea surface height (SSH) at unprecedented spatial resolution, and this comes with a lot of scientific and technical challenges. One of them is that at scales <100km, SWOT SSH data will not only contain signatures of large scale currents, mesoscale eddies and fronts but also signatures of internal tides. We therefore need to get ready for analysing and filtering these geophysical signals.   

Ocean model simulations are a **key source of information for preparing the upcoming SWOT altimeter mission**. They provide virtual realizations of the data that the SWOT mission will flux when it flies. These virtual observations are used for preparing the algorithms that will massage the raw SWOT data in order to get meaningfull information on ocean circulation. But meeting this objective requires that ocean model simulations describe as realistically as possible oceanic motions at the scales that will be sampled by the mission. 

Over the last few years, our group has put a lot of effort in **producing, analysing and sharing model data from a North Atlantic model** configuration based on [NEMO](https://www.nemo-ocean.eu/) ocean model code base and called [NATL60](https://meom-group.github.io/swot-natl60/). With their 1/60° horizontal resolution and 300 vertical levels, our series of NATL60 model simulations have proven to be very useful for preparing SWOT mission. But they also have their caveats : the runs were rather short, the domain did not cover the whole North Atlantic basin. Most importantly, the simulations **did not account for internal tides**...  

This is why we teamed up with Ocean Next and put together a 40M CPU hours computing ressource proposal to [PRACE](http://www.prace-ri.eu) last year. The proposal was successful and we therefore got into this **challenge of producing tide-resolving, submesoscale permitting, basin scale ocean simulations** with this configuration called **eNATL60**. The simulation programme was probably one of the largest ever simulation programme performed with an ocean model. And this actually went on pretty smoothly thanks to the years of work by NEMO System Team for including tides in NEMO and thanks to the great people who provided advise at each stage of the model design and run production.  

Last week, just a couple of days after the end of the run production, Laurent Brodeau presented the first results of the simulations at [OceanPredict'19](http://oceanpredict19.org/). He showed in particular how the **simulated SSH signals closely follow observations** from present day altimeters (like the AltiKa-SARAL mission). His analysis also show this very specific shallowing of SSH wavenumber spectra in models that resolve internal tides as illustrated below.    

![image]({{site.baseurl}}/img/image_com_PSD_SSH_Azores_season.png "eNATL60 comparison with AltiKa-SARAL altimeter data")

But I guess the real challenge is actually only starting now. We have indeed produced **1.5Pb (!!) of ocean model data** with our twin runs (with and without tides). Both the size of the dataset and the number of scientific questions we can adress with it are pretty overwhelming.... But there are good news : 

 - *Good news #1* :  the french computing infrastructure **[GENCI](http://www.genci.fr) and the [CINES](https://www.cines.fr) national center have kindly accepted to store the data** close to one of the largest french supercomputers; 

 - *Good news #2* : the **[PANGEO](https://pangeo.io/) community provides a great software stack** for analysing these data.  


Final word, as for the NATL60 data, **eNATL60 model data are opened to anybody willing analyse them**, just contact us through email if you want to access the data. Laurent Brodeau has posted several nice hi-res animations of the model output on [Ocean Next vimeo channel](https://vimeo.com/oceannext) if you want to get a more precise idea of what you could do with this dataset.   

[![image]({{site.baseurl}}/img/vimeo-channel-oceannext.png "eNATL60 videos on vimeo")](https://vimeo.com/oceannext)







