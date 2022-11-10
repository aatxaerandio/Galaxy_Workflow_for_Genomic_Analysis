[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
# Galaxy Workflow for bacterial genomes 
## Introduction
This practical aims to guide you to perform tasks such as importing data, working with histories, running your analysis and downloading your results. This tutorial is for those who are newbies in genomics and bioinformatics, in order to ease the analysis of WGS data.
This Galaxy Workflow for WGS data aims to perform an automated and complete characterization of bacterial genomes including; genome annotation, species identification, serotype prediction, antimicrobial resistance prediction, virulence-related genes and plasmid replicon detection, core-genome-based or single nucleotide polymorphism (SNP)-based phylogenetic clustering and sequence typing. 
## Installation
No installation steps are required, just download the [Galaxy Workflow]( https://github.com/aatxaerandio/Galaxy_Workflow_for_Genomic_Analysis/blob/main/Genomic%20Analysis%20Workflow.ga) file and upload to your personal Galaxy account.
## Requirements
To run this practical workflow for bacterial WGS data you will need:
1. An internet-connected computer with a compatible web browser such as Firefox, Chrome or Safari.
2. Access to a Galaxy instance. In our case, we choose the [European Galaxy server](https://usegalaxy.eu/).
## Tutorial
# Prior to your analysis
<img align="right" src="https://user-images.githubusercontent.com/75436856/201067360-4e49565c-2714-4ded-8cd1-381cdcb2b111.png">
In your selected browser, go to the https://usegalaxy.eu/ and log in or register. 
The Galaxy web interface is composed by three main parts; i) A wide variety of tools available to perform your desired analysis, ii) a central panel that shows the home page where you will be able customize your parameters and see dataset contents, and iii) the analysis history on the right containing the analysis performed on your dataset. 
Before analysing your WGS data: (1) workflow must be [downloaded]( https://github.com/aatxaerandio/Galaxy_Workflow_for_Genomic_Analysis/blob/main/Genomic%20Analysis%20Workflow.ga) and imported to your Galaxy account; (2) Data must be uploaded. 

1. Move to Workflows on the top menu bar of Galaxy and click on the upload icon Galaxy-upload at the top right of the screen. Upload the workflow file in the box labelled “Archived Workflow File” and click the Import workflow button.
2. After importing the workflow, data to be analysed must be provided. By default, a the “unnamed history” is available. History and dataset´s name can be modified to your wills. Name your histories or/and datasets to be meaningful and easy to find by clicking on the :pencil2: icon. Do not forget of saving your edit. Click on the “Upload data” button located on the left side of the browser. There are several ways to upload your data to Galaxy. We recommend uploading your data in “Regular” by dropping the files in the central panel or clicking on “choose local files” and selecting the desired files. Click on “Start” and files will be uploaded sequentially. Once uploaded, they will appear on your history, on the right side of the browser. On your history, click on :heavy_check_mark: icon to select items and click on the selected bar. Many options will be displayed. 
If your history is composed by contig files, you can click on “Build Dataset List” to create a dataset containing all the selected items. On the contrary, if your history is composed by pair end reads, you can select them and click on “Build List of Dataset Pairs”, to make pairs of forward and reverse reads and group pairs on a dataset. By building list we ensure that all the elements are analysed once the workflow is executed. 
# Launch your analysis
Once the workflow is uploaded and your data is “built”, it is time to launch the analysis. 
Click on Workflow on the top bar and click on play :arrow_forward: icon. Here select the reference genome and the input dataset collection. If you wish, you can customize workflow´s tools parameters to your need as well as sending the results to other history.
Click on Run Workflow and all jobs will be scheduled and executed.
 ![imagen](https://user-images.githubusercontent.com/75436856/201067326-bca7c884-4ba9-4a39-91b1-452b52fc14b8.png)
# After your analysis
Check your history to see if your analysis went well. It will go through different statuses before is completed. 
| Colour | Icon | Meaning | Status |
| --------- | ----------- |  ----------- |  ----------- |
| Grey | Clock | Job is running | ![imagen](https://user-images.githubusercontent.com/75436856/201066965-c7e31267-1337-4767-a522-37b3ca6a1698.png) |
| Yellow | Spinner | Dataset element is waiting to start | ![imagen](https://user-images.githubusercontent.com/75436856/201067118-50635c99-e0f0-4763-9e65-8afd21f698e1.png) |
| Green | None | Job is finished | ![imagen](https://user-images.githubusercontent.com/75436856/201067180-a2a998ff-c033-4b1a-bd03-94ab085cf99b.png) |
| Red | Cross | Job has failed | ![imagen](https://user-images.githubusercontent.com/75436856/201067155-6eba1b29-4871-410e-b630-da7408248df9.png) |
Once the dataset is green, click and it will expand the dataset to see a preview containing general information about it. For further information, click on the Galaxy-eye (OJO) icon and dataset information will be displayed in the central panel. Info regarding tool parameters can be checked clicking on :information_source:.
In case the job has failed, you can rerun the job by clicking on :leftwards_arrow_with_hook: icon. Check carefully each tool´s required inputs and formats to avoid unwelcomed failed Jobs. 
For downloading the results, click on the :floppy_disk: icon available when dataset information is displayed in your history.
## Output Files
By running this workflow, several output files will be created. Here we highlight the main results:
* Raw read trimming and quality reports
* Species identification with Krona charts
* Assembly and assembly statistics 
* Sequence typing (Multi Locus Sequence Typing)
* Strain serotype
* AMR and virulence gene detection
* Plasmid replicon detection
* Genome Annotation files (see [prokka outputs](https://github.com/tseemann/prokka#output-files)).
* Core gene alignment and core genome-based clustering
* SNP detection and SNP-based clustering
* SNP distance matrix
## Test
You can test run with files in /test data (web)
## Troubleshooting
Submit problems or requests to the [Issue Tracker](https://github.com/aatxaerandio/Galaxy_Workflow_for_Genomic_Analysis/issues) or check [Galaxy Help pages](https://help.galaxyproject.org/).
