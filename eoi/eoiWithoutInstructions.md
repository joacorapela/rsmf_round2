Start here
==========

Category
--------

RSMF Round 2

Application name
----------------

Consolidating Bonsai as a Standard for Neuroscience Intelligent
Experimental Control

Research Area
-------------

Biological, Medical and Veterinary Sciences

Eligibility
===========

Software to be maintained
-------------------------

Bonsai

Programming language
--------------------

C\#

Software maturity and UK research benefit
-----------------------------------------

Bonsai is used by multiple research laboratories at many UK
institutions, like UCL, Francis Crick Institute and MRC Laboratory of
Molecular Biology. It was created in 2012 and has more than 28 public
releases. Please refer to the [releases listing in
GitHub](https://github.com/bonsai-rx/bonsai/releases).

Bonsai allows to create issues and provide feedback through the Issues
and Discussion sections of its [GitHub
repository](https://github.com/bonsai-rx/bonsai). Contributions can be
made by opening pull requests, as indicated in its [Contribution
Guide](https://bonsai-rx.org/contribute/). In addition, Bonsai has its
own package manager and most often Bonsai users contribute to the
ecosystem by creating Bonsai packages, as explained in the
[documentation](https://bonsai-rx.org/docs/articles/create-package.html).

Lead organisation
-----------------

Sainsbury Wellcome Centre, University College London

Vision and impact
=================

Motivation, Vision and Impact
-----------------------------

### Motivation

Bonsai[^1] is a software ecosystem used by thousands of (mostly
experimental neuroscience) users in the UK and all around the world
(7,000 downloads per year and 1,000 citations per year of the core
Bonsai paper [Lopes et al., 2015]). Being a visual-programming language,
Bonsai allows scientists with little programming experience to control
sophisticated neuroscience experiments.

Machine learning (ML) is now essential for most branches of science,
neuroscience in particular. Yet, current neuroscience experiments are
still controlled by simple means (e.g., deliver a reward when a rat
pokes left but not right). In 2022, we realised that adding ML
functionality to Bonsai could empower Bonsai users and enable a
radically new type of intelligent experimental control. We created the
Bonsai.ML[^2] package providing machine learning functionality to the
Bonsai ecosystem. Bonsai.ML now contains packages to characterise animal
behaviour (e.g., [Linear Dynamical
Systems](https://bonsai-rx.org/machinelearning/articles/LinearDynamicalSystems/lds-overview.html)
and [Hidden Markov
Model](https://bonsai-rx.org/machinelearning/articles/HiddenMarkovModels/hmm-overview.html)
packages) and to decode behavioural features from neural activity (e.g.,
[Point Process
Decoder](https://bonsai-rx.org/machinelearning/articles/PointProcessDecoder/ppd-overview.html)
package). And we will soon add a new Neural Latents package to infer low
dimensional representations of high-channel-count neural recordings [as
in Yu et al., 2009]. Bonsai.ML interacts with ML packages written in Python
using the [Python Scripting](https://bonsai-rx.org/python-scripting/)
package, and with PyTorch functionality using the [Torch
package](https://bonsai-rx.org/machinelearning/articles/Torch/torch-overview.html).

However, since most experimental neuroscientists currently using Bonsai
are not skilled in ML, we need to invest extra efforts on
**documentation, training and community building** to help them make the
most of the Bonsai.ML package. In addition, to improve the
**maintainability and efficiency** we will implement all inference
methods of Bonsai.ML in a state-of-the-art C\# probabilistic programming
language.

### Relevance to the UK Research Ecosystem

Bonsai has established itself as mission-critical infrastructure within
the UK's world-leading neuroscience and behavioural research
communities. Its adoption is widespread across premier institutions; at
[University College London (UCL)](https://www.ucl.ac.uk/) alone, it is
utilised by more than ten research groups at the [Sainsbury Wellcome
Centre](https://www.sainsburywellcome.org/), as well as the [Cortex
Lab](https://www.ucl.ac.uk/brain-sciences/cortexlab), the [Coen
Lab](https://coen-lab.com/), and the [Institute for Behavioural
Neuroscience](https://www.ibn.ucl.ac.uk/).

The framework's reach extends across UK centres of excellence, including
the [Kinetic Cognition Lab](https://www.tripodilab.org/) at the [MRC
Laboratory of Molecular Biology](https://www2.mrc-lmb.cam.ac.uk/) and
the [Znamenskiy
Lab](https://www.crick.ac.uk/research/labs/petr-znamenskiy) at the
[Francis Crick Institute](https://www.crick.ac.uk/).

By consolidating Bonsai.ML functionality, this proposal will unlock
advanced real-time computational power for these groups, transforming
how high-dimensional neural data is processed and directly catalysing
new scientific discoveries across the UK research landscape.

### Relation to experimental control software ecosystem

The experimental control landscape is currently fragmented between
rigid, domain-specific interfaces (e.g., [Open
Ephys](https://open-ephys.org), [Miniscope
DAQ](https://github.com/Aharoni-Lab/Miniscope-DAQ-Software)) and
specialised task-logic frameworks (e.g.,
[pyControl](https://pycontrol.readthedocs.io/),
[Autopilot](https://autopilot-docs.readthedocs.io/), [NIMH
ML](https://monkeylogic.nimh.nih.gov/)). While general programming in
[Python](https://www.python.org/) or
[MATLAB](https://www.mathworks.com/products/matlab.html) offers total
flexibility, it remains high-maintenance and largely inaccessible to
non-expert programmers.

[Bonsai](https://bonsai-rx.org/) disrupts this trade-off by offering a
free and open-source, high-level visual syntax that combines the
accessibility of a GUI with the modular extensibility of a full
programming language. Unlike expensive, closed-source alternatives like
[LabVIEW](https://www.ni.com/en-us/shop/labview.html)---which suffer
from overly granular and complex logic structures---Bonsai enables
researchers to design and successfully customise sophisticated,
multi-device experiments rapidly from the ground up, regardless of prior
coding expertise.

Benefits
--------

The proposed activities will empower the UK research community to
integrate sophisticated Machine Learning (ML) into Bonsai workflows,
driving unprecedented neuroscientific discoveries. The defining
achievement of Bonsai's reactive visual programming is its ability to
collapse the gap between conceptual design and experimental
execution. It enables domain experts to rapidly architect
high-complexity, multi-device experiments---tasks that would typically
require a dedicated programmer days to develop, if achievable at all.

While most ML frameworks are designed for offline, disk-based
processing, Bonsai.ML uniquely enables real-time, online
processing within closed-loop architectures. This transition from
post-hoc analysis to live experimental control has two transformative
implications:

1.  **For Neuroscientists:** It provides a novel toolkit for real-time
    data interaction, enabling the discovery of brain functions
    observable only during active, closed-loop manipulation.

2.  **For ML Developers:** By providing a robust stream of real-time
    neural and behavioural data, Bonsai serves as a premier platform to
    validate and deploy algorithms in live environments.

Though focused on neuroscience, Bonsai.ML will impact other UK
sectors, including robotics and interactive art. Ultimately, this
project demonstrates a fundamental paradigm shift: graphical
programming is an unparalleled mechanism for putting advanced
computational functionality---historically gatekept by expert software
engineers---directly into the hands of domain experts. By removing
complex code syntax, Bonsai allows researchers to architect
sophisticated systems at the speed of thought, significantly multiplying
the innovation potential and research velocity of the UK's scientific
workforce.

EDIA
----

We are committed to ensuring that Bonsai.ML is accessible, inclusive,
and beneficial to the widest possible community of neuroscience
researchers.

The Bonsai.ML team itself is diverse, with leadership from Croatia,
India, and Portugal, and research software engineers from Argentina and
Canada. This diversity shapes our perspective and makes us strong
advocates of EDIA. Bonsai already has a global user base spanning all
five continents. It empowers researchers in disadvantaged communities,
notably in Eastern Europe and South America. A recent example is the
[Transatlantic Behavioural Neuroscience School (Argentina, August
2025)](https://nenckiopenlab.org/tbns2025/), where Bonsai was used to
enable cutting-edge training opportunities across borders.

At its core, Bonsai embodies inclusivity: it allows non-programmers to
design and run sophisticated experiments. This lowers barriers for
researchers from underrepresented groups, smaller institutions, or
disciplines outside computer science---broadening participation in
methods that would otherwise remain the preserve of elite or technically
specialised groups. With Bonsai.ML, we extend this philosophy by
providing non-programmers with state-of-the-art ML tools.

The activities supported by this grant will further embed EDIA
principles. Comprehensive documentation and training will lower entry
barriers through step-by-step tutorials, plain-language explanations,
captioned video materials, and diverse experimental examples. Our
documentation approach will closely follow the `scikit-learn` project,
which is internationally recognised for embracing EDIA principles
through clarity, consistency, and accessible contribution pathways.
Finally, community events such as the 2026 Bonsai Developers Conference
will adopt a code of conduct, select a diverse range of speakers across
career stages, genders, and regions, and provide hybrid participation
options to reduce financial and travel barriers.

Feasibility and Approach
========================

Proposed work
-------------

To maximise the impact, long-term sustainability and maintainability of
Bonsai.ML, this proposal pursues seven aims:

1.  **Documentation** -- Produce comprehensive, user-centred
    documentation that makes ML tools accessible to non-specialists
    across the neuroscience community. This documentation will follow
    the [scikit-learn](https://scikit-learn.org) model.

2.  **Training** -- Develop and deliver a practical training course on
    Bonsai and Bonsai.ML, building capacity and lowering barriers to
    adoption, as in [previous Bonsai
    courses](https://bonsai-rx.org/learn/).

3.  **Dissemination** -- Publish the first Bonsai.ML paper to increase
    visibility and uptake within the scientific community.

4.  **Maintainability** -- In collaboration with Microsoft Research
    Cambridge, integrate their C\# probabilistic programming library
    *Infer.NET* into Bonsai.ML. This will simplify and unify inference
    and learning code, making it faster, more maintainable, and more
    extensible, while embedding the expertise of a world-leading
    industrial research group into the Bonsai ecosystem.

5.  **Community reach** -- Engage neuroscientists interested in
    *closed-loop* neural experimentation by supporting the use of
    [CLOCTools](https://cloctools.github.io/) within Bonsai.ML, in
    collaboration with Prof. Garrett Stanley (Georgia Tech). This
    partnership will attract a new community of researchers to Bonsai
    and broaden its reach to an emerging but underrepresented area of
    neuroscience.

6.  **Community building** -- Strengthen the developer community by
    organising the second Bonsai Developers Conference in December 2026,
    building on the successful [inaugural event in
    2024](https://conference.bonsai-rx.org/2024/).

7.  **Governance** -- Establish a steering committee to guide a
    long-term roadmap and prioritise sustainability.

By the end of the funding period, Bonsai.ML will provide high-quality
documentation and training resources, a robust and maintainable
codebase, and a stronger developer community with expanded expertise and
broader reach. In particular, collaborations with Microsoft Research
Cambridge and Prof. Garrett Stanley's laboratory will embed cutting-edge
knowledge in probabilistic inference and closed-loop experimentation.
Together, these efforts will ensure Bonsai remains a sustainable,
maintainable, and widely adopted research software platform, aligned
with UKRI's strategic priorities in artificial intelligence, bioscience,
and community-driven research software sustainability.

### Measures of impact

We are currently using the measures described below to assess the impact
of Bonsai in the experimental neuroscience and/or methods development
community. We will compare the change of these measures before and after
each project milestone is achieved.

**Bonsai.ML nuget package downloads**: we monitor the number of Bonsai.ML package downloads at <https://www.nuget.org/packages/Bonsai.ML>,

**Number of Bonsai packages integrated into Bonsai.ML**: we use nuget.org to check the number of packages that are using Bonsai.ML at <https://www.nuget.org/packages/Bonsai.ML>, which is a proxy to the number of methods developers contributing to Bonsai.ML.

**Bonsai.ML discussions in Bonsai forum**: we track discussions in the Bonsai forum that are related to Bonsai.ML (e.g., <https://github.com/orgs/bonsai-rx/discussions?discussions_q=is%3Aopen+bonsai.ml>.

**Usage of <https://github.com/bonsai-rx/machinelearning>**: we observe the stars/watching/clones of this repository

**Citations to the forthcoming Bonsai.ML paper**.

Software sustainability
-----------------------

Bonsai.ML will be sustained beyond the RSMF funding period through a
combination of community, institutional, and commercial support.
NeuroGEARS, which already underpins the wider Bonsai ecosystem, invests
a fixed proportion of its service income into Bonsai maintenance and
will extend this support to Bonsai.ML.

Our academic partners are also strongly invested. The Sainsbury Wellcome
Centre (SWC) relies on Bonsai for experimental control and Bonsai.ML for
advanced control in some of its experiments, and contributes financially
to its development. The Gatsby Unit will continue to provide machine
learning expertise to guide Bonsai.ML's growth. Prof. Stanley's lab will
contribute its expertise in the control of physiological signals to
extend Bonsai.ML's capabilities.

Finally, our collaboration with Microsoft Research Cambridge ensures
that Infer.NET integration brings sustained industrial expertise to
Bonsai.ML, strengthening its long-term sustainability beyond the funding
period.

Capability to Deliver
=====================

Delivery team and mechanisms
----------------------------

This proposal is led by a multidisciplinary team of world-class experts
across the Sainsbury Wellcome Centre (SWC), the Gatsby Computational
Neuroscience Unit, and NeuroGEARS Ltd. The team integrates high-level
institutional leadership with deep technical expertise in ML, reactive
programming, and experimental neuroscience.

### Leadership and Technical Team

-   **Prof. Thomas Mrsic-Flogel (Project Lead, SWC):** Director of the
    SWC and founding member of the International Brain Laboratory (IBL).
    He brings extensive experience in systems neuroscience, managing
    large-scale, reproducible neuroscience infrastructure and led the
    BBSRC project that established Bonsai.ML.

-   **Prof. Maneesh Sahani (Co-Lead, Gatsby Unit):** A pioneer in
    computational neuroscience. His research provided the mathematical
    backbone for population-scale neural analysis globally. He co-led
    the foundational Bonsai.ML project and provides theoretical guidance
    for disseminating advanced ML tools.

-   **Dr. Gonçalo Lopes (Co-Lead, NeuroGEARS):** The creator of Bonsai.
    With a background in computer sciences, he directs NeuroGEARS, the
    non-profit engine driving the core development of the Bonsai visual
    programming language.

-   **Dr. Joaquín Rapela (RSE, Gatsby Unit):** A specialist in
    probabilistic ML and signal processing with industry experience at
    IBM. He is the lead developer of svGPFA and has spearheaded the
    technical development of Bonsai.ML since its inception.

-   **Dr. Nicholas Guilbeault (RSE, NeuroGEARS):** With a background in
    biology, he has ample experience in closed-loop stimulation and
    reactive software development. Previously the developer of *BonZeb*,
    he serves as the core developer for the Bonsai.ML project,
    integrating ML methods into the reactive framework.

### Synergy and Community Engagement

The team's skills are balanced across ML, software engineering, and
experimental control, complemented by project partners including Tom
Minka (probabilistic inference; Microsoft Research) and Josh Siegle
(electrophysiology and large-scale neuroscientific software development
and distribution; Allen Institute).

Bonsai thrives on a decentralised sustainability model. While NeuroGEARS
maintains the core, over 70% of its 130+ packages are
community-contributed. This "distributed maintenance" prevents single
points of failure and ensures the software evolves alongside scientific
discovery.

Several channels exist to engage Bonsai users in the development
process. First, Bonsai uses [GitHub
Discussions](https://github.com/orgs/bonsai-rx/discussions) and a
[Discord Server](https://discord.gg/FB5MSKgh) for daily interactions.
Second, there is a weekly Bonsai Dev Club, open to the public, where
Bonsai developers meet to discuss the latest Bonsai development issues
(notes from these meetings appear
[here](https://github.com/orgs/bonsai-rx/discussions/categories/dev-club)).
Third, for more than ten years NeuroGEARS has been delivering two or
more [Bonsai courses](https://bonsai-rx.org/learn/) every year at major
universities. Fourth, every two years Bonsai users can join the [Bonsai
Developer Conference](https://conference.bonsai-rx.org/2024/), where
Bonsai users and developers meet for a one-week-long presentations about
the latest Bonsai developments and shape the Bonsai development plan.

### Sustainability and Development Standards

Bonsai adheres to rigorous software engineering practices, including
modular architecture, automated unit testing, and semantic versioning to
ensure backward compatibility. Supported by the Bonsai Foundation CIC,
the platform is engineered for long-term resilience. By fostering a
cohort of "Scientist-Developers," we reduce reliance on closed-source
commercial software. These practices ensure that Bonsai remains a
transparent and sovereign research infrastructure for the UK and
international scientific communities.

[^1]: <https://bonsai-rx.org/>

[^2]: <https://bonsai-rx.org/machinelearning>
