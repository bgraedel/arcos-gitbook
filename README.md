---
description: ARCOS - Automated Recognition of Correlated Structures
---

# ARCOS

![](https://github.com/user-attachments/assets/c643eeb2-1425-4d0a-812f-21bbb2282c0f)

## About

ARCOS is a computational method to detect and quantify collective, spatio-temporally correlated phenomena. The algorithm identifies and tracks spatial clusters in time-lapse images. Although designed to analyze signalling phenomena in biological cells or cell collectives, it is applicable to other systems even outside of the realm of cell biology.



<figure><img src=".gitbook/assets/erk-waves-mdck-2rows.gif" alt=""><figcaption></figcaption></figure>

## Code

We provide open-source implementations of ARCOS for:

* [Python](https://github.com/bgraedel/arcos4py)
* [R](https://github.com/dmattek/ARCOS)

Both code bases can handle segmented data and raster images, although the Python version contains additional optimizations and features to handle large datasets.

## GUI

Additionally, two dedicated interactive plugins for [napari image viewer](https://napari.org/stable/) are available:

* [arcos-gui](https://github.com/bgraedel/arcos-gui) − to handle data from image segmentation
* [arcosPx-napari](https://github.com/bgraedel/arcosPx-napari) − to handle raster images

The napari plugins enables anyone without extensive programming knowledge to explore parameters through an intuitive GUI on a platform that emerges as a de-facto standard for viewing multidimensional images.

## Demos

* Demo of the arcos-gui napari plugin ([YouTube](https://youtu.be/hG_z_BFcAiQ))
* Demo of the entire workflow from raw images to detection of collective events ([YouTube](https://youtu.be/vVDYst-1SyM?si=wk3fnatOTQc4bMn5))

## Publications

The original ARCOS algorithm is now published in the Journal of Cell Biology (JCB):\
[https://doi.org/10.1083/jcb.202207048](https://doi.org/10.1083/jcb.202207048)

For a complete tutorial on how to use ARCOS from raw images to full analysis refer to our publication in Methods in Microscopy (MiM):\
[https://doi.org/10.1515/mim-2024-0003](https://doi.org/10.1515/mim-2024-0003)

and the corresponding [GitHub repository](https://github.com/dmattek/ARCOS-tutorial) containing a detailed notebook and installation instructions.

If you use this method in your research, please cite our papers:

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
    issn = {0021-9525},
    doi = {10.1083/jcb.202207048},
    url = {https://doi.org/10.1083/jcb.202207048},
}
```

and if you used the tutorial please also cite:

```
@article{arcos-tutorial-2024,
    author = {Dobrzyński, Maciej and Grädel, Benjamin and Gagliardi, Paolo Armando and Pertz, Olivier},
    title = {Quantification of collective signalling in time-lapse microscopy images},
    journal = {Methods in Microscopy},
    volume = {1},
    number = {1},
    pages = {19--30},
    year = {2024},
    month = {06},
    issn = {2942-3899},
    doi = {doi:10.1515/mim-2024-0003},
    url = {https://doi.org/10.1515/mim-2024-0003},
}
```

## How to use ARCOS

{% content-ref url="example-use-cases/detecting-collective-signalling-events-in-epithelial-cells.md" %}
[detecting-collective-signalling-events-in-epithelial-cells.md](example-use-cases/detecting-collective-signalling-events-in-epithelial-cells.md)
{% endcontent-ref %}

{% content-ref url="example-use-cases/analysing-collective-phenomena-in-honeybees.md" %}
[analysing-collective-phenomena-in-honeybees.md](example-use-cases/analysing-collective-phenomena-in-honeybees.md)
{% endcontent-ref %}

## How ARCOS works

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
