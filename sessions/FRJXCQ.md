---
layout: session
title: "Investigating the capability of UAV imagery in AI-assisted mapping of Refugee Camps in East Africa"
code: "FRJXCQ"
speaker_names: ['Christopher Chan']
affiliations: None
room: "Auditorium B"
length: "5"
time: "Sunday, 10:40"
time_iso: "2022-08-21T08:40:00Z"
resources: []
recording: True
---

This pilot project is connected to a larger initiative to open-source the assisted mapping platform for Humanitarian OpenStreetMap (HOTOSM) based on Very High Resolution (VHR) drone imagery. The study test and evaluate multiple U-Net based architectures on building segmentation of Refugee Camps in East Africa.

<hr>

Introduction

Refugee camps and informal settlements provide accomodation to some of
the most vulnerable population, the majority of which are located in Sub-
Saharan East Africa (UNHCR, 2016). Many of these settlements often lack
up-to-date maps of which we take for granted in developed settlements. Hav-
ing up-to-date maps are important for assisting administration tasks such as
population estimates and infrastructure development in data impoverished
environments, and thereby encourages economic productivity (Herfort et al.,
2021). The data inequality between the developed and developing countries
are often resulted from a lack of commercial interest, especially with the
recent trend of corporate OSM mappers (Anderson et al., 2019, Veselovsky
et al., 2021). Such disparity can be reduced using assisted mapping tech-
nology. To extract geospatial and imagery characteristics of dense urban
enviornments, a combination of VHR satellite imagery and Machine Learn-
ing (ML) are commonly used (Taubenböck et al., 2018). Classical ML based
methods that exploit the textual (e.g. GLCM), spectral, and morphological
characteristics of VHR imagery are based on the principles of Computer
Vision (CV). Although many have shown promising results in satellite VHR
(1m to 5m resolution) scenarios such as differentiating slum and non-slum
(Kuffer et al., 2016 &amp; Wurm et al., 2021), in VHR drone imagery (5cm to
10cm resolution) however, results might suffer from noise caused by environ-
ment and drone-based specific problems such as motion artefacts and litter.
Recent advances in CV based Deep Learning might be able to address these
issues (Chen et al., 2021 &amp; Carrivick et al., 2016).

Purpose of the study

The study is connected to a larger initiative to open-source the assisted
mapping platform in the current Humanitarian OpenStreetMap (HOTOSM)
ecosystem. This study is a pilot-project to investigate the capabilities of
applying semantic segmentation using community open-sourced VHR drone
imagery collected by the partner organisation OpenAerialMap. The study
aims to rigourosly assess the various components and inputs that would
contribute to the ML based mapping system, and to produce a detailed
evaluation on class-based accuracy assessment (Congalton &amp; Green, 2019).
This pilot study focuses on 2 camps in East Africa, where data availability
and the geography of the camps are within a similar savannah ecosystem.
This enables highly-detailed method testing and analysis of transferability
of the results between the two camps.

Data and Methodology

The first camp is located in Dzaleka, Dowa, Malawi, which is sub-divided
into the Dzaleka North and Dzaleka main camp. The Dzaleka camps are
home to around 40,000 refugees mainly coming from the African Great Lakes
region. The Dzaleka North camp is characterised by a newer, spatially well-
planned metal-sheeted roofs, while the southern main camp is characterised
by complex, dense mud-walled building with stone-lined thatched-roofs (UN-
HCR, 2014). The second camp, the Kalobeyei settlement is part of the sub-
camp of Kakuma, located in the rural county of Turkana, North-West Kenya.
The Kalobeyei settlement was home to approximately 34,849 refugees as of
2019. This camp is significantly more spacious and is characterised by spa-
tiall well-planned metal-sheeted roofs (UNHCR &amp; DANIDA, 2019). VHR
drone imageries were provided for both camps and vector labels produced
by HOTOSM volunteers were provided for the Dzaleka and Dzaleka North
camp.

Since CV based Deep Learning is very dependent on the quality of the
labelled referenced data, especially when performing pixel-based semantic
segmentaion, it is of crucial importance that care is taken when producing
highly accurate labels that ensure sucessful training (Ng A., 2018). A large
quanitiy of available labels did not have such a task in mind, imperfection
in labelling around existing drone artefacts could cause the trained model
to misclassify such pixels. In order to train a model which performs well
on drone imagery, the motion artefact will be a signficant feature for the
model to learn.he combination of data availability have allow a unique set of
research questions concerning the input data quality and experiment setup
to surface. Therefore, to test out U-Net and a few variation of the U-Net
performance, an additional set of label data was created in order to supple-
ment the imperfection in the labelled data of the Dzaleka camps. Initially,
the models will be trained on the pixel-perfect and less complex Kalobeyei
dataset, this will be then be followed by introducing the Dzaleka datasets
of higher complexity. A comparison of baseline performance between the U-
Net variations (Ronneberger et al., 2015) and the Open-Cities-AI-Challenge
(OCC) winning model is conducted. The baseline experiement aims to keep
the hyperparameters (e.g. optimiser, learning rate, weight decay etc.) con-
stant to obtain an objective view of the architectual responses on the same
dataset setup. This will provide a clear picture of the feasibility and how to
take this project further, so that further resources could be justified to scale
future experiments.

Findings and Discussion

Initial baseline experiments on the Kalobeyei dataset and Kalobeyei with
the Dzaleka(s) seem to suggest limited transferability from the OCC model.
This suggests that the OCC model is perhaps over-generalised to the compe-
tition test dataset. Despite achieving very high confidence on metal-sheeted
rooftops, it does not detect any of the more complicated thatched roofs com-
mon in the Dzaleka camp. The OCC model also struggle with
some of the more obscure drone motion artefacts occuring at the edge of the
imagery in the Kalobeyei camp. Meanwhile, the Precision and Recall statis-
tics favour other variations or further transfer training on the OCC model,
and the EfficientNet B1 header U-Net pretrained with ImageNet weights.
However validation loss suggests there might be little room for improvement
in the further transfer training of the OCC model.

Precision and Recall have both reached above 0.7 in most experiments,
which outline the general capability of the strategies used. However there
are still significant variations among different architectures and setups. The
next step is to perform systemic fine-tuning to increase the confidence level
of the appropriate architectures.

<hr>

Anderson, J., Sarkar, D., &amp; Palen, L. (2019). Corporate Editors in the Evolving Landscape of OpenStreetMap. ISPRS International Journal of Geo-Information, 8(5), 232. https://doi.org/10.3390/ijgi8050232
Carrivick, J. L., Smith, M. W., &amp; Quincey, D. J. (2016). Structure from Motion in the Geosciences. John Wiley &amp; Sons.
Congalton, R. G., &amp; Green, K. (2019). Assessing the accuracy of remotely sensed data: Principles and practices (3rd ed.). CRC press.
Dzaleka Refugee Camp. (2017, June 8). There Is Hope. http://thereishopemalawi.org/dzaleka-refugee-camp/
Herfort, B., Lautenbach, S., de Albuquerque, J. P., Anderson, J., &amp; Zipf, A. (2021). The evolution of humanitarian mapping within the OpenStreetMap community. Scientific Reports, 11(1), 1–15.
Kuffer, M., Pfeffer, K., Sliuzas, R., &amp; Baud, I. (2016). Extraction of Slum Areas From VHR Imagery Using GLCM Variance. IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, 9(5), 1830–1840. https://doi.org/10.1109/JSTARS.2016.2538563
Minghini, M., Ludwig, C., Anderson, J., Mooney, P., &amp; Grinberger, A. Y. (2021). Proceedings of the Academic Track at State of the Map 2021. Zenodo. https://doi.org/10.5281/zenodo.5116434
Ng, A. (2018). Machine Learning Yearning.
Open Cities AI Challenge: Segmenting Buildings for Disaster Resilience. (2022). [Jupyter Notebook]. DrivenData. https://github.com/drivendataorg/open-cities-ai-challenge (Original work published 2020)
Ronneberger, O., Fischer, P., &amp; Brox, T. (2015). U-Net: Convolutional Networks for Biomedical Image Segmentation. In N. Navab, J. Hornegger, W. M. Wells, &amp; A. F. Frangi (Eds.), Medical Image Computing and Computer-Assisted Intervention – MICCAI 2015 (pp. 234–241). Springer International Publishing. https://doi.org/10.1007/978-3-319-24574-4_28
Taubenböck, H., Kraff, N. J., &amp; Wurm, M. (2018). The morphology of the Arrival City—A global categorization based on literature surveys and remotely sensed data. Applied Geography, 92, 150–167. https://doi.org/10.1016/j.apgeog.2018.02.002
UNHCR. (2014). Malawi: Joint Assessment Mission Report. Dzaleka Refugee Camp (November 2014) (WFP/UNHCR/GOM/PRDO/JRS/PLAN). UNHCR. https://www.unhcr.org/protection/health/5680f7d09/malawi-joint-assessment-mission-report-dzaleka-refugee-camp-november-2014.html
UNHCR &amp; DANIDA. (2019). The Integrated Solutions Model in and Around Kalobeyei, Turkana, Kenya (No. 978-87-93760-22–6). UNHCR, DANIDA. https://www.unhcr.org/research/evalreports/5dfa287c4/unhcrdanida-integrated-solutions-model-around-kalobeyei-turkana-kenya.html
UNHCR Sub-Office Kakuma. (2019). Kakuman camp and Kalobeyei Settlement Briefing Kit, May 2019.
Wurm, M., Weigand, M., Schmitt, A., Geiß, C., &amp; Taubenböck, H. (2017). Exploitation of textural and morphological image features in Sentinel-2A data for slum mapping. 2017 Joint Urban Remote Sensing Event (JURSE), 1–4. https://doi.org/10.1109/JURSE.2017.7924586

