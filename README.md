# artifacts-of-llmgendata
This repository contains scripts for running the experiments illustrated in the paper:
> *"Under the Surface: Tracking the Artifactuality of LLM-Generated Data"*<br>
Debarati Das<sup>†¶</sup>, Karin de Langis<sup>¶</sup>, Anna Martin-Boyle<sup>¶</sup>, Jaehyung Kim<sup>¶</sup>, Minhwa Lee<sup>¶</sup>, Zae Myung Kim<sup>¶</sup>, Shirley Anugrah Hayati, Risako Owan, Bin Hu, Ritik Sachin Parkar, Ryan Koo, Jong Inn Park, Aahan Tyagi, Libby Ferland, Sanjali Roy, Vincent Liu, Dongyeop Kang<br>
Minnesota NLP, University of Minnesota Twin Cities<br>
<sup>†</sup> Project Lead, <sup>¶</sup> Core Contribution <br>

*Our website can be accessed at this [Link](https://minnesotanlp.github.io/artifact/).*
*The paper can be accessed at [arXiv](https://arxiv.org/pdf/2401.14698.pdf).*<br>
*The datasets used in the paper can be downloaded from [HuggingFace Hub](https://huggingface.co/datasets/minnesotanlp/LLM-Artifacts).*

## Overview
This research project collects diverse text data from large language models (LLMs), encompassing both structured "task labels" and open-ended "free-form text." This extensive dataset allows for a holistic examination of LLM outputs, offering insights into their performance under varying degrees of structure and freedom. The research underscores the importance of responsible and ethical practices in LLM-generated data creation and usage, advocating for collaborative efforts to address biases, enhance diversity, and deepen the understanding of complex human opinions in LLM outputs for ethical and sustainable development.

The structure of the repository closely follows the stress testing methods applied to the five different data types: *Task Labels*, *Preferences*, *Instructions*, *Simulations*, and *Free-Form Text*

More specifically, the stress testing experiments are categorized as either "first-order" or "second-order" experiments. In short, the first-order experiments investigate the data "as-is," for example, focusing on their distributional differences and correlation patterns among human- and LLM-generated data; validating and analyzing using manual inspection; and counting how often labels flip between the original human and the resulting machine text. The second-order experiments involve fine-tuning LLMs on the machine-generated data and investigating whether the existing artifacts or biases are amplified.

<img width="1588" alt="image" src="https://github.com/minnesotanlp/artifacts-of-llmgendata/assets/3746478/ae37ef70-78fe-4142-8cc5-8eb02a2c8efd">

<br>

*The code for the corresponding first-order and second-order experiments are placed under two directories of the same names, respectively, except for Simulation data type where we did not perform a second-order experiment.*

Under each data type directory, a corresponding `README.md` file is located for further details:
- [Task Labels](https://github.com/minnesotanlp/artifacts-of-llmgendata/tree/main/task_labels)
- [Preferences](https://github.com/minnesotanlp/artifacts-of-llmgendata/tree/main/preference)
- [Instructions](https://github.com/minnesotanlp/artifacts-of-llmgendata/tree/main/instructions)
- [Simulations](https://github.com/minnesotanlp/artifacts-of-llmgendata/tree/main/simulation)
- [Free-Form Text](https://github.com/minnesotanlp/artifacts-of-llmgendata/tree/main/free_form_text)

## Citation
```
@misc{das2024surface,
  title={Under the Surface: Tracking the Artifactuality of LLM-Generated Data}, 
  author={Debarati Das and Karin De Langis and Anna Martin and Jaehyung Kim and Minhwa Lee and Zae Myung Kim and Shirley Hayati and Risako Owan and Bin Hu and Ritik Parkar and Ryan Koo and Jonginn Park and Aahan Tyagi and Libby Ferland and Sanjali Roy and Vincent Liu and Dongyeop Kang},
  year={2024},
  eprint={2401.14698},
  archivePrefix={arXiv},
  primaryClass={cs.CL}
}
```
