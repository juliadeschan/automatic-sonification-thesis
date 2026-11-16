1. Detect scientific articles based on the existence of a doi
2. Check browser extensions for scientific articles, e.g. Forrt ORE
3. Identify literature via HTML metadata, **TODO**: Need Regex check in content as well?
4. Identifying figures based on tag "figure" not all inclusive, e.g. https://doi.org/10.1146/annurev-orgpsych-031424-094816
5. TODO: Determine all-inclusive way for figure detection
   1. Chosen approach: scan through figure types assume that if the figure type gives results thats what the publisher chose
6. TODO: Determine way to handle figures that include multiple plot
7. Issue: Some figures don't get the buttons. -> extended the figure detection to more than just figure
8. Issue: It reconised the figures navigation as a figure and added sonify/interact to that navigation bar -> fixed for specific next of kin div types
9. Issue: Leaving the extension running in the background creates more and more buttons