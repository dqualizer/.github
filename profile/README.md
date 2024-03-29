# dqualizer

## Goal
The dqualizer project enables domain-driven runtime quality analysis (RQA) of software systems by leveraging Domain Driven Design techniques. In particular, dqualizer focuses on domain-driven monitoring, load testing, and resilience testing.
For more information, please visit our [website](https://dqualizer.github.io/).

## Overview

![dqarchitecture-en3-1](https://user-images.githubusercontent.com/18191871/224370639-2b793379-6727-465a-bbd6-fd46a9326c11.png)

The dqualizer approach consists of six components with different responsibilities: 

| **Component** | **Short Description** |
|---------------|-----------------------|
| [dqualizer](https://github.com/dqualizer/dqualizer)   | The main repository contains elements that are related to all components, e.g., documentation.  |
| [dqanalyzer](https://github.com/dqualizer/dqanalyzer2)   | The dqanalyzer component enables domain experts to specify and perform RQA without profound knowledge of the underlying technical infrastructure and analysis tools.  |
| [dqcockpit](https://github.com/dqualizer/dqcockpit)   |  Dqcockpit is a dashboard visualizing the results of executed RQAs. |
| [dqedit](https://github.com/dqualizer/dqedit)   | The dqedit component is the editor for the mapping necessary to translate domain questions / RQA definitions to technical RQA configurations. |
| [dqtranslator](https://github.com/dqualizer/dqtranslator)   | Dqtranslator maps (domain) RQA definitions to technical RQA configurations that can be executed by dqexec. It also maps the technical results back to the domain level. |
| [dqexec](https://github.com/dqualizer/dqexec)   |  The dqexec component executes the RQA configuration by utilizing state-of-the-art monitoring, load testing, and resilience testing tooling. |
| [dqlang](https://github.com/dqualizer/dqlang)   | The dqlang is a collection of languages utilized by dqualizer e.g., the DST extension for domain-level RQA specification or the language for defining mappings in dqedit. |
| [dqapi](https://github.com/dqualizer/dqapi)   | The dqapi is a REST Api, which is responsible to execute CRUD Operations on different dqualizer artifacts. It is used to manage RQAs and DAMs in the mongoDB.  |

For a detailed description of the architecture, we refer to our [arc42 document](https://dqualizer.github.io/dqualizer). 

## Cite
If you want to refer to dqualizer in scientific papers, please use the following publication:

    @proceedings{dqualizer23,
      title        = "dqualizer: Domain-Centric Runtime Quality Analysis of Business-Critical Application Systems",
      authors      = "Frank, Sebastian and Brott, Julian and Kesim, Dominik and Holz, Heiko and Eschhold, Matthias and van Hoorn, André"
      year         = "2023",
      booktitle    = "Companion of the 2023 ACM/SPEC International Conference on Performance Engineering (ICPE '23 Companion)",
      doi          = "10.1145/3578245.3584853",
      publisher    = "ACM"
    }

