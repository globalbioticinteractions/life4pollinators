[![GloBI review by Elton](https://github.com/globalbioticinteractions/life4pollinators/actions/workflows/review.yml/badge.svg)](https://github.com/globalbioticinteractions/life4pollinators/actions) [![GloBI](http://api.globalbioticinteractions.org/interaction.svg?accordingTo=globi:globalbioticinteractions/life4pollinators)](http://globalbioticinteractions.org/?accordingTo=globi:globalbioticinteractions/life4pollinators) 

Configuration for Global Biotic Interactions (GloBI, https://globalbioticinteractions.org) to help index insect-flower interactions associated with the Barberis, M., Bitonto, F. F., Costantino, R., Bianco, L., Birtele, D., Bonifacino, M., Cangelmi, G., Capó, M., Chroni, A., d'Agostino, M., Dal Cin, M., Devalez, J., Bortolotti, L., Flaminio, S., Giacò, A., Lenzi, L., Magagnoli, S., Minici, A., Nakas, G., … Galloni, M. (2025). Insect-flower interactions in the Mediterranean area: a Citizen Science dataset collated within the LIFE 4 Pollinators project [Data set]. Zenodo. https://doi.org/10.5281/zenodo.16949654 

See also:

Barberis, M., Bitonto, F. F., Costantino, R., Bianco, L., Birtele, D., Bonifacino, M., … Galloni, M. (2025). Insect-flower interactions in the Mediterranean area: a Citizen Science dataset collated within the LIFE 4 Pollinators project. Journal of Pollination Ecology, 39, 306–315. https://doi.org/10.26786/1920-7603(2025)872

## Curatorial Notes

As published in https://doi.org/10.5281/zenodo.16949654, ```LIFE 4 Pollinators Darwin Core.zip``` (hash://md5/2ee4f59c1b481c6e564ba41b6459983e) was edited to better conform with DwC-A: 

1. Character encoding - The meta.xml suggested that UTF-8 encoding was used. However, UTF-16 encoding was found. The updated meta.xml now sets the encoding to UTF-16 as expected. 
2. delimiters - the meta.xml suggested that semi-colons were used as delimiters. However, in the data tables, tab separated values are found. The meta.xml was updated to reflect this.
3. merging two occurrence tables - in original dataset, two occurrence tables were found: ```plants.txt``` and ```flower visitors.txt```. The two occurrence tables were merged to ```occurrence.tsv``` and the meta.xml was updated accordingly.
4. mismatched event id and occurrence id values - for some reason, the original datasets included some event id prefixes that had no equivalent in the ```event.txt``` table. These included:  

from ```flower visitor.txt```

eventID | occurrenceID | scientificName | occurrenceRemarks
--- | --- | --- | ---
LIFE4POLL828e | LIFE4POLL828e-a-1002188 | Rhagonycha sp. | uncertain
LIFE4POLL828f | LIFE4POLL828f-a-1002189 | Rhagonycha sp. | uncertain
LIFE4POLL828h | LIFE4POLL828h-a-1002191 | Rhagonycha sp. | uncertain
LIFE4POLL828i | LIFE4POLL828i-a-1002192 | Rhagonycha sp. | uncertain
LIFE4POLL828l | LIFE4POLL828l-a-1002193 | Rhagonycha sp. | uncertain
LIFE4POLL828m | LIFE4POLL828m-a-1002194 | Rhagonycha sp. | uncertain
LIFE4POLL828n | LIFE4POLL828n-a-1002195 | Rhagonycha sp. | uncertain
LIFE4POLL828o | LIFE4POLL828o-a-1002196 | Rhagonycha sp. | uncertain

The event id prefixes were truncated to exclude the letter suffix. For example ```LIFE4POLL828e``` was changed to ```LIFE4POLL828```.

The authors and editors of the Journal of Pollination Ecology has been notified on 2026-03-24. 
