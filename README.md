---
description: ARCOS - Automated recognition of collective signalling events
---

# ARCOS



ARCOS is a computational method to detect and quantify collective phenomena. The algorithm was designed with the signaling of epithelial cells in mind however it is also applicable to other systems even outside of the realm of cell biology.&#x20;

We provide several open-source implementations of ARCOS

* [Python](https://github.com/bgraedel/arcos4py) (arcos4py)
* [R ](https://github.com/dmattek/ARCOS)[ ](https://github.com/bgraedel/arcos4py)(ARCOS)
* [Plugin for Napari image viewer](https://github.com/bgraedel/arcos-gui) (arcos-gui)

ARCOS is now published in the Journal of Cell Biology (JCB):\
&#x20;[https://doi.org/10.1083/jcb.202207048](https://doi.org/10.1083/jcb.202207048)

For a complete tutorial on how to use ARCOS from raw images to full analysis you may also refer to our recent tutorial published in Methods in Microscopy (MiM):\
[https://doi.org/10.1515/mim-2024-0003](https://doi.org/10.1515/mim-2024-0003)

and the corresponding [GitHub repository containing a detailed notebook and installation instructions](https://github.com/dmattek/ARCOS-tutorial).

## Detecting Collective events with ARCOS

<div align="center">

<img src=".gitbook/assets/export(1).gif" alt="Quantification of a collective signaling event in a MDCK epithelium. Credit Paolo Gagliardi">

</div>

### How to get ARCOS

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

### How to use ARCOS

{% content-ref url="example-use-cases/detecting-collective-signalling-events-in-epithelial-cells.md" %}
[detecting-collective-signalling-events-in-epithelial-cells.md](example-use-cases/detecting-collective-signalling-events-in-epithelial-cells.md)
{% endcontent-ref %}

{% content-ref url="example-use-cases/analysing-collective-phenomena-in-honeybees.md" %}
[analysing-collective-phenomena-in-honeybees.md](example-use-cases/analysing-collective-phenomena-in-honeybees.md)
{% endcontent-ref %}

### Overview of how ARCOS works

Learn the fundamentals of ARCOS to get a deeper understanding of our main features:

{% content-ref url="algorithm-overview/event-detection-and-tracking.md" %}
[event-detection-and-tracking.md](algorithm-overview/event-detection-and-tracking.md)
{% endcontent-ref %}

{% content-ref url="algorithm-overview/data-requirements.md" %}
[data-requirements.md](algorithm-overview/data-requirements.md)
{% endcontent-ref %}

{% content-ref url="algorithm-overview/preprocessing.md" %}
[preprocessing.md](algorithm-overview/preprocessing.md)
{% endcontent-ref %}

If you use this method in your research, please cite our paper:

```
@article{10.1083/jcb.202207048,
    author = {Gagliardi, Paolo Armando and Grädel, Benjamin and Jacques, Marc-Antoine and Hinderling, Lucien and Ender, Pascal and Cohen, Andrew R. and Kastberger, Gerald and Pertz, Olivier and Dobrzyński, Maciej},
    title = "{Automatic detection of spatio-temporal signaling patterns in cell collectives}",
    journal = {Journal of Cell Biology},
    volume = {222},
    number = {10},
    pages = {e202207048},
    year = {2023},
    month = {07},
    abstract = "{Increasing experimental evidence points to the physiological importance of space–time correlations in signaling of cell collectives. From wound healing to epithelial homeostasis to morphogenesis, coordinated activation of biomolecules between cells allows the collectives to perform more complex tasks and to better tackle environmental challenges. To capture this information exchange and to advance new theories of emergent phenomena, we created ARCOS, a computational method to detect and quantify collective signaling. We demonstrate ARCOS on cell and organism collectives with space–time correlations on different scales in 2D and 3D. We made a new observation that oncogenic mutations in the MAPK/ERK and PIK3CA/Akt pathways of MCF10A epithelial cells hyperstimulate intercellular ERK activity waves that are largely dependent on matrix metalloproteinase intercellular signaling. ARCOS is open-source and available as R and Python packages. It also includes a plugin for the napari image viewer to interactively quantify collective phenomena without prior programming experience.}",
    issn = {0021-9525},
    doi = {10.1083/jcb.202207048},
    url = {https://doi.org/10.1083/jcb.202207048},
    eprint = {https://rupress.org/jcb/article-pdf/222/10/e202207048/1915749/jcb\_202207048.pdf},
}
```

and if you used the tutorial please also cite:

```
@article{DobrzyńskiGrädelGagliardiPertz+2024,
    url = {https://doi.org/10.1515/mim-2024-0003},
    title = {Quantification of collective signalling in time-lapse microscopy images},
    title = {},
    author = {Maciej Dobrzyński and Benjamin Grädel and Paolo Armando Gagliardi and Olivier Pertz},
    journal = {Methods in Microscopy},
    doi = {doi:10.1515/mim-2024-0003},
    year = {2024},
    lastchecked = {2024-06-18}
}
```
