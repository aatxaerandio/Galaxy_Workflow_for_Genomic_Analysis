[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)


# Galaxy Workflow for Genomic Analysis
Galaxy Workflow to perform an automated and complete characterization of bacterial genomes

# Launch your analysis
Once the workflow is uploaded and your data is “built”, it is time to launch the analysis. 
Click on Workflow on the top bar and click on play (icon) icon. Here select the reference genome and the input dataset collection. If you wish, you can customize workflow´s tools parameters to your need as well as sending the results to other history.
Click on Run Workflow and all jobs will be scheduled and executed.
 

# After your analysis
Check your history to see if your analysis went well. It will go through different statuses before is completed. 
| Colour | Icon | Meaning | Status |
| --------- | ----------- |  ----------- |  ----------- |
| Grey | Clock | Job is running | Status |
| Yellow | Spinner | Dataset element is waiting to start | Status |
| Green | None | Job is finished | Status |
| Red | Cross | Job has failed | Status |

Once the dataset is green, click and it will expand the dataset to see a preview containing general information about it. For further information, click on the Galaxy-eye (OJO) icon and dataset information will be displayed in the central panel. Info regarding tool parameters can be checked clicking on :information_source:.
In case the job has failed, you can rerun the job by clickin on :leftwards_arrow_with_hook: icon. Check carefully each tool´s required inputs and formats to avoid unwelcomed failed Jobs. 
For downloading the results, clik on the :floppy_disk: icon available when dataset information is displayes in your history.

## Output Files
By running this workflow, several output files will be created. Here we highlight the main results:
Raw read trimming and quality reports
Species identification with Krona charts
Assembly and assembly statistics 
Sequence typing (Multi Locus Sequence Typing)
Strain serotype
AMR and virulence gene detection
Plasmid replicon detection
Genome Annotation files (see prokka output (https://github.com/tseemann/prokka#output-files)).
Core gene aligment and core genome-based clustering
SNP detection and SNP-based clustering
SNP distance matrix
