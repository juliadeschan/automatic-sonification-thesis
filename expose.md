# Exposé: 
Automatic Data Recovery and Interactive Sonification for Screen-Reader Accessibility of Scientific Visualisations

## 1. Background and Context
<p>PDF is currently one of the most common formats for scientific publications. However, PDFs can pose significant accessibility challenges for blind and low-vision (BLV) readers, particularly when used with screen readers (Wang et al. 2021). Screen readers are a primary tool used by BLV researchers to access scientific literature (Katsnelson 2023), making the accessibility of scientific publications an important issue for accessible scientific communication.</p>
<p>One approach to improving accessibility is to provide scientific publications in tagged HTML in addition to PDF or to convert existing publications into HTML. Screen readers generally work well with appropriately structured HTML documents. One tool following this approach is SciA11y, which converts scientific PDFs into tagged HTML and enables interactive screen-reader-based access to their contents (Wang et al. 2021). The tool demonstrates the potential of integrating accessible scientific literature more directly into the workflow of BLV researchers. However, SciA11y and similar approaches still face difficulties with certain types of content, particularly tables, figures, and mathematical formulas (Wang et al. 2021).</p>
<p>This thesis focuses specifically on the accessibility of scientific figures. A straightforward approach would be to provide alternative text for figures. However, alternative text for scientific figures is often insufficient or poorly implemented (Wang et al. 2021). More importantly, textual descriptions alone limit the ability of BLV researchers to independently explore the data the same way as is possible when represented by a visualisation.</p>
<p>Sonification offers a possible approach to this problem. Sonification is defined by Hermann et al. (2011) as “the data-dependent generation of sound, if the transformation is systematic, objective and reproducible”. It can be used to represent data through auditory properties such as pitch, duration, rhythm, or spatialisation, allowing users to explore relationships and patterns in data without relying on visual representations. Sonification is already used by BLV researchers as a means of exploring and analysing data (Katsnelson 2023).</p>
<p>However, scientific publications introduce an additional challenge: the complete dataset underlying a visualisation is often not available in the publication itself. Instead, a figure may only provide a visual representation of the data. The data therefore needs to be recovered from the figure before it can be sonified. Several approaches for automated chart-data recovery have been proposed, with much of the existing research focusing on the development and evaluation of methods for machine learning and computer vision applications. One such approach is ChartRecover by Yuan et al. (2026), a deep-learning framework for recovering data from scientific charts. ChartRecover supports [insert specific chart types] and is designed to reconstruct the data represented in a visual chart. [Insert brief explanation of how ChartRecover works and its performance.]</p>
<p>While ChartRecover is only one possible approach to chart-data recovery, its ability to reconstruct data from visualisations makes it potentially useful for the proposed application. This thesis therefore explores whether existing chart-data recovery methods can be combined with sonification to support the accessible exploration of scientific figures.</p>

## 2. Research Problem and Motivation
<p>Existing approaches to accessible scientific publications can improve access to textual content, but scientific figures remain a significant challenge. Alternative text can communicate information about a figure, but it does not necessarily provide access to the relationships and patterns within the represented data.</p>
<p>At the same time, sonification provides established methods for representing data through sound and can support data exploration without visual input. Automated chart-data recovery could provide the data necessary for such sonification even when the original dataset is not included in the publication.</p>
<p>The proposed thesis therefore investigates the combination of these approaches. The goal is to develop an interactive system that enables BLV researchers to access and explore data represented in scientific publications through sonification. The exact scope and workflow of the system, including whether individual figures or entire scientific articles can be processed, will be determined based on the identified requirements, existing approaches, and technical feasibility.</p>

## 3. Aim of the Thesis
<p>The aim of this thesis is to design and implement a browser-based interactive system that enables BLV researchers to explore data represented in scientific publications through sonification. The system will combine automated data recovery from scientific figures with interactive sonification and may be integrated into an article-level workflow in which textual content and figures are made accessible together. The exact scope and functionality will be determined based on identified requirements and technical feasibility.</p>
<p>Potential features include automatic sonification, interaction, and saving sonifications or their configurations for later use.</p>

## 4. Research Question
<p>Potential research questions include:</p>

1. How can we implement an accessibility tool for BLV researchers to interactively explore data represented in scientific figures?
2. How can we design an interactive browser-based sonification tool to enable BLV users to explore scientific figures and publications?
3. How can we automatically recover and transform data from scientific figures into interactive sonifications?
4. How can we support the interactive exploration of data represented in scientific figures by BLV researchers using automatically generated sonification?
5. How can we support BLV researchers in interactively exploring data represented in scientific figures through an accessible browser-based system?
6. How can we support support BLV researchers in exploring both textual and visual information in scientific publications using an accessible browser-based workflow?

## 5. Preliminary Literature
Hermann, T., Hunt, A., & Neuhoff, J. G. (2011). *The sonification handbook*. Logos Verlag. 

Katsnelson, A. (2023, March 6). *These tools help visually impaired scientists read data and journals.* Nature News. https://www.nature.com/articles/d41586-023-00645-6 

Wang, L. L., Cachola, I., Bragg, J., Cheng, E. Y.-Y., Haupt, C., Latzke, M., Kuehl, B., van Zuylen, M. N., Wagner, L., & Weld, D. (2021). SCIA11Y: Converting scientific papers to accessible HTML. *Proceedings of the 23rd International ACM SIGACCESS Conference on Computers and Accessibility, 1–4.* https://doi.org/10.1145/3441852.3476545 

Yuan, Y., Liang, S., Zhang, J., Wang, Y., & Wang, Z. (2026). A deep learning framework for scientific chart data extraction and Reconstruction. *Communications Engineering*, 5(1). https://doi.org/10.1038/s44172-026-00691-8 