# Overview 

- [00.OverviewPapers.md](Overview Papers)

# Contributions to Activities of the SDLC

- [./01.Planning.md](1. Planning)
- [./02.Analysis.md](2. Analysis)
- [./03.Design.md](3. Design)
- [./04.Implementation.md](4. Implementation)
- [./05.Testing.md](5. Testing and Integration)
- [./06.Maintenance.md](6. Maintenance)


## 5. Testing & Integration

### [Automated Unit Test Improvement using Large Language Models at Meta](https://arxiv.org/abs/2402.09171)

> This paper describes Meta's TestGen-LLM tool, which uses LLMs to automatically improve existing human-written tests. TestGen-LLM verifies that its generated test classes successfully clear a set of filters that assure measurable improvement over the original test suite, thereby eliminating problems due to LLM hallucination. We describe the deployment of TestGen-LLM at Meta test-a-thons for the Instagram and Facebook platforms. In an evaluation on Reels and Stories products for Instagram, 75% of TestGen-LLM's test cases built correctly, 57% passed reliably, and 25% increased coverage. During Meta's Instagram and Facebook test-a-thons, it improved 11.5% of all classes to which it was applied, with 73% of its recommendations being accepted for production deployment by Meta software engineers. We believe this is the first report on industrial scale deployment of LLM-generated code backed by such assurances of code improvement.

### [Software Testing with Large Language Models: Survey, Landscape, and Vision](https://arxiv.org/abs/2307.07221)

> Pre-trained large language models (LLMs) have recently emerged as a breakthrough technology in natural language processing and artificial intelligence, with the ability to handle large-scale datasets and exhibit remarkable performance across a wide range of tasks. Meanwhile, software testing is a crucial undertaking that serves as a cornerstone for ensuring the quality and reliability of software products. As the scope and complexity of software systems continue to grow, the need for more effective software testing techniques becomes increasingly urgent, making it an area ripe for innovative approaches such as the use of LLMs. This paper provides a comprehensive review of the utilization of LLMs in software testing. It analyzes 102 relevant studies that have used LLMs for software testing, from both the software testing and LLMs perspectives. The paper presents a detailed discussion of the software testing tasks for which LLMs are commonly used, among which test case preparation and program repair are the most representative. It also analyzes the commonly used LLMs, the types of prompt engineering that are employed, as well as the accompanied techniques with these LLMs. It also summarizes the key challenges and potential opportunities in this direction. This work can serve as a roadmap for future research in this area, highlighting potential avenues for exploration, and identifying gaps in our current understanding of the use of LLMs in software testing.

### [Quickly generating diverse valid test inputs with reinforcement learning](https://par.nsf.gov/servlets/purl/10172516)

> Property-based testing is a popular approach for validating the logic of a program. An effective property-based test quickly generates many diverse valid test inputs and runs them through a parameterized test driver. However, when the test driver requires strict validity constraints on the inputs, completely random input generation fails to generate enough valid inputs. Existing approaches to solving this problem rely on whitebox or greybox information collected by instrumenting the input generator and/or test driver. However, collecting such information reduces the speed at which tests can be executed. In this paper, we propose and study a black-box approach for generating valid test inputs. We first formalize the problem of guiding random input generators towards producing a diverse set of valid inputs. This formalization highlights the role of a guide which governs the space of choices within a random input generator. We then propose a solution based on reinforcement learning (RL), using a tabular, on-policy RL approach to guide the generator. We evaluate this approach, RLCheck, against pure random input generation as well as a state-of-the-art greybox evolutionary algorithm, on four real-world benchmarks. We find that in the same time budget, RLCheck generates an order of magnitude more diverse valid inputs than the baselines.

### [CODAMOSA: Escaping coverage plateaus in test generation with pre-trained large language models](https://www.carolemieux.com/codamosa_icse23.pdf)

> Search-based software testing (SBST) generates high-coverage test cases for programs under test with a combination of test case generation and mutation. SBST’s performance relies on there being a reasonable probability of generating test cases that exercise the core logic of the program under test. Given such test cases, SBST can then explore the space around them to exercise various parts of the program. This paper explores whether Large Language Models (LLMs) of code, such as OpenAI’s Codex, can be used to help SBST’s exploration. Our proposed algorithm, CODAMOSA, conducts SBST until its coverage improvements stall, then asks Codex to provide example test cases for under-covered functions. These examples help SBST redirect its search to more useful areas of the search space. On an evaluation over 486 benchmarks, CODAMOSA achieves statistically significantly higher coverage on many more benchmarks (173 and 279) than it reduces coverage on (10 and 4), compared to SBST and LLM-only baselines.

### [Flakify: A black-box, language model-based predictor for flaky tests](https://ieeexplore.ieee.org/abstract/document/9866550?casa_token=h59HzsagJQcAAAAA:6Pyb6-smpaAQm7P2rVvJly2qp--3c80w-NbDeL8sz3i0vO_wfHhYmp0Yzrw0bddRybVwDOJmsw)

> Software testing assures that code changes do not adversely affect existing functionality. However, a test case can be flaky, i.e., passing and failing across executions, even for the same version of the source code. Flaky test cases introduce overhead to software development as they can lead to unnecessary attempts to debug production or testing code. Besides rerunning test cases multiple times, which is time-consuming and computationally expensive, flaky test cases can be predicted using machine learning (ML) models, thus reducing the wasted cost of re-running and debugging these test cases. However, the state-of-the-art ML-based flaky test case predictors rely on pre-defined sets of features that are either project-specific, i.e., inapplicable to other projects, or require access to production code, which is not always available to software test engineers. Moreover, given the non-deterministic behavior of flaky test cases, it can be challenging to determine a complete set of features that could potentially be associated with test flakiness. Therefore, in this article, we propose Flakify, a black-box, language model-based predictor for flaky test cases. Flakify relies exclusively on the source code of test cases, thus not requiring to (a) access to production code (black-box), (b) rerun test cases, (c) pre-define features. To this end, we employed CodeBERT, a pre-trained language model, and fine-tuned it to predict flaky test cases using the source code of test cases. We evaluated Flakify on two publicly available datasets (FlakeFlagger and IDoFT) for flaky test cases and compared our technique with the FlakeFlagger approach, the best state-of-the-art ML-based, white-box predictor for flaky test cases, using two different evaluation procedures: (1) cross-validation and (2) per-project validation, i.e., prediction on new projects. Flakify achieved F1-scores of 79% and 73% on the FlakeFlagger dataset using cross-validation and per-project validation, respectively. Similarly, Flakify achieved F1-scores of 98% and 89% on the IDoFT dataset using the two validation procedures, respectively. Further, Flakify surpassed FlakeFlagger by 10 and 18 percentage points (pp) in terms of precision and recall, respectively, when evaluated on the FlakeFlagger dataset, thus reducing the cost bound to be wasted on unnecessarily debugging test cases and production code by the same percentages (corresponding to reduction rates of 25% and 64%). Flakify also achieved significantly higher prediction results when used to predict test cases on new projects, suggesting better generalizability over FlakeFlagger. Our results further show that a black-box version of FlakeFlagger is not a viable option for predicting flaky test cases.


## 6. Maintenance

# Prompt Engineering

- [Best practices for prompt engineering with OpenAI](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api)
- [Learning Performance-Improving Code Edits](https://arxiv.org/abs/2304.11384)


# Unsorted
- [Teaching large language models to self-debug](https://arxiv.org/abs/2304.05128)
- 

