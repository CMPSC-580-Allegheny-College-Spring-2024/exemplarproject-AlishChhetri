[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/Y4rZMh1t)
# Junior Seminar (CMPSC 580) Exemplar Project Repository

## Semester: Spring 2024

This repository contains student project materials, including project report, data, code, and references to literature for this departmentally-sponsored project. __As you complete each of the below sections in this document, please be sure to remove the preamble text so that it does not appear in your work.__ Please work with your first reader to answer any questions or concerns that you may have.

## GitHub Handle: AlishChhetri

## Name: Alish Chhetri

## Major: Software Engineering

## Project Name: COMMA

![Comma Logo](image.png)

"COMMA" stands for "Chasten Output Mutmut Mutation Analysis" 

---

## Overview

<!-- TODO (250 words minimum): Discuss the overview of the project using and building on the project description provided by the department. In this section, a concise summary is discussed of the study's key elements, offering the reader a quick understanding of the research's scope and goals. The section continues to outline the main topics, research questions, hypotheses, and /or theories in a clear and meaningful language to provide a type of roadmap for the reader to navigate the forthcoming details of the project. This section also needs to motivate the project by providing context for the study, outlining the current state of knowledge in the field, and highlighting any gaps or limitations in existing research. The section serves as a foundational guide that enables the reader to grasp the context of the study, in addition to its structure, before moving into a more technically-based discussion in the following sections of the article. In short, the "Overview" section needs to answer the `what` and `why` questions, that is `what is the project?` and `why is the project important?` -->

The project aims to investigate the relationship between code quality anti-patterns and mutation scores in Python programs, building on prior research that demonstrated such correlations in Java programs. Mutation testing, a technique for evaluating the effectiveness of test suites by introducing defects into a program and assessing whether they are detected, serves as the central focus. Despite its potential to enhance software testing practices, mutation testing is underutilized due to its computational demands. Therefore, this research seeks to address this gap by developing a predictive tool that can estimate mutation scores shortly after the implementation of test cases, providing software engineers with early insights into the effectiveness of their test suites.

The study's primary objectives include identifying code quality anti-patterns prevalent in Python programs and examining their impact on mutation scores. By doing so, the research aims to contribute to the improvement of software testing methodologies and the overall quality of software development processes. This project's significance lies in its potential to empower software engineers with tools and knowledge to enhance the effectiveness of their testing strategies, ultimately leading to more robust and reliable software systems.

Furthermore, this project fills a notable gap in empirical research by extending the investigation of code quality anti-patterns and mutation scores beyond the Java programming language to Python. By broadening the scope of inquiry, this research expands the understanding of software quality assurance practices across different programming paradigms, thereby enriching the body of knowledge in the field.

## Literature Review

<!-- TODO: Conduct literature review by describing relevant work related to the project and hence providing an overview of the state of the art in the area of the project. This section serves to contextualize the study within the existing body of literature, presenting a thorough review of relevant prior research and scholarly contributions. In clear and meaningful language, this section aims to demonstrate the problems, gaps, controversies, or unanswered questions that are associated with the current understanding of the topic. In addition, this section serves to highlight the current study's unique contribution to the field. By summarizing and critiquing existing works, this section provides a foundation for readers to appreciate the novelty and significance of the study in relation to the broader academic discourse. The "Literature Review" section further contributes to the `why is the project important?` question. The number of scholarly work included in the literature review may vary depending on the project. -->

[Jia2011](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects/blob/main/software-engineering/paper-pdfs/Jia2011.pdf):

The paper provides a comprehensive analysis and survey of Mutation Testing, a fault-based software testing technique, spanning over three decades of research. It highlights the growing interest and maturity of Mutation Testing, evidenced by rapid developments in tools, techniques, and applications across various programming languages and domains. Recent efforts focus on reducing the cost of Mutation Testing without compromising its effectiveness, leading to successful techniques for optimizing the testing process. Additionally, there is a trend towards more elaborate forms of mutation, emphasizing semantic effects over syntactic achievements. This shift indicates a maturation of the field, with an increasing focus on generating realistic mutants and developing practical tooling to support comprehensive testing efforts. Overall, the findings suggest that Mutation Testing is reaching a mature state, poised for further advancements in detecting subtle faults and improving overall software quality.

[Spadini2018](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects/blob/main/software-engineering/paper-pdfs/Spadini2018.pdf):

This paper investigates the impact of test smells, sub-optimal design choices in test code, on software quality. Through an analysis of over a million test cases from ten software systems, the study reveals that tests affected by smells are more change- and defect-prone, with certain smells such as 'Indirect Testing', 'Eager Test', and 'Assertion Roulette' being particularly significant. The findings indicate a negative association between test smells and test code quality, with smelly tests exhibiting a higher risk of defects and change-proneness compared to non-smelly tests. Moreover, the presence of test smells correlates with higher defect-proneness in the tested production code, suggesting a potential impact on overall software quality. The study emphasizes the need for further research and the development of automated test smell detection tools to improve the effectiveness of testing processes and enhance software quality. Overall, it underscores the importance of addressing test smells to mitigate their adverse effects on software maintenance and defect detection.

[Virginio2019](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects/blob/main/software-engineering/paper-pdfs/Virginio2019.pdf):

This study investigates the relationship between test smells and test coverage, aiming to enhance software quality assurance practices. Test smells, indicators of issues in test code affecting maintainability, are analyzed alongside test coverage metrics using the JNose Test tool across eleven open-source projects. The findings reveal correlations between test smells and test coverage, suggesting that test smells may influence code coverage. Specifically, the Lazy Test emerges as a prevalent test smell, often indicating challenges in test maintenance. The analysis yields 210 correlations, indicating varying degrees of association between test smells and test coverage metrics. While four strong correlations and 17 moderate correlations are identified, 147 pairs show no correlation. Future work entails a deeper exploration of these correlations, expanding the study to diverse projects, refining the JNose Test algorithm, and identifying code segments most affected by test smells. Overall, the study provides insights that can aid software testers in understanding the impact of poorly designed tests on software quality and maintenance.

[Wang2021](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects/blob/main/software-engineering/paper-pdfs/Wang2021.pdf):

This paper addresses the lack of automated tools for detecting test smells in Python, despite its increasing popularity. By extending research to Python and developing a tool called PYNOSE, the authors aim to identify and analyze test smells in Python projects. They gather a list of 17 diverse test smells from existing research and introduce a new test smell called Suboptimal Assert, identified through mining frequent code change patterns. PYNOSE, implemented as a plugin to PyCharm, is capable of detecting these test smells with high precision and recall. Empirical analysis on a dataset of 450 open-source Python projects reveals that 98% of projects and 84% of test suites contain at least one test smell, with Suboptimal Assert being detected in 70.6% of projects. Overall, the study provides valuable insights into the prevalence of test smells in Python code and the effectiveness of PYNOSE in detecting them, highlighting the importance of addressing test smells to improve software quality in Python projects.

[Zhu2021](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects/blob/main/software-engineering/paper-pdfs/Zhu2021.pdf):

This paper introduces a new perspective for software developers to understand and address low mutation scores by considering testability and observability metrics. Investigating correlations between these metrics and mutation scores across six open-source Java projects, the study reveals a significant correlation between observability metrics and mutation scores, particularly emphasizing factors like test directness. Leveraging insights from this correlation, the paper proposes "mutation score anti-patterns" to guide developers in refactoring existing code or enhancing test suites to improve mutation scores. By conducting a manual analysis of methods with low mutation scores and applying anti-pattern-based refactorings, the study demonstrates the potential effectiveness of these approaches in increasing mutation scores. However, the paper acknowledges the trade-offs involved in certain refactorings, such as violating object-oriented design principles. Therefore, developers are encouraged to carefully consider options like adding test cases, refactoring production code, or ignoring surviving mutants, while weighing the trade-offs between design principles and testability/observability. Overall, the paper contributes newly proposed code observability metrics, insights into the relationship between testability/observability metrics and mutation scores, a case study illustrating the impact of anti-pattern removal on mutation scores, and guidelines for developers facing low mutation scores. Additionally, a prototype tool called Mutation Observer is provided to automate the calculation of code observability metrics, aiding developers in their decision-making process.

Why our project is important:

Our project is crucial within the context of existing research due to its focus on providing developers with actionable insights when confronted with low mutation scores. While previous studies have extensively explored mutation testing, test smells, and their impact on software quality, our work introduces a novel perspective by considering testability and observability metrics. By investigating correlations between these metrics and mutation scores across various open-source Java projects, we aim to shed light on the factors influencing mutation scores and provide developers with practical guidance on improving them. Building upon insights from existing literature, such as the correlation between test smells and software quality, our project proposes "mutation score anti-patterns" to help developers refactor code or enhance test suites to boost mutation scores effectively. Moreover, our study emphasizes the importance of considering trade-offs between design principles and testability/observability when making decisions to address low mutation scores. By offering a comprehensive approach that integrates insights from diverse research streams and providing a prototype tool called Mutation Observer to automate the calculation of code observability metrics, our project seeks to empower developers with the necessary tools and knowledge to enhance software quality through mutation testing.

## Methods

<!-- TODO: Discuss the methods of the project to be able to answer the `how` question (`how was this project completed?`). The methods section in an academic research outlines the specific procedures, techniques, and methodologies employed to conduct the study, offering a transparent and replicable framework for the research. It details the resources behind the work, in terms of, for example, the design of the algorithm and the experiment(s), data collection methods, applied software libraries, required tools, the types of statistical analyses and models which are applied to ensure the rigor and validity of the study. This section provides clarity for other researchers to understand and potentially replicate the study, contributing to the overall reliability and credibility of the research findings. -->

This research project employs a systematic approach to investigate the relationship between code quality anti-patterns and mutation scores for Python projects. The following methods outline the procedures, tools, and analyses used to address the research questions:

Subject Program Collection: Python programs meeting specific criteria, including the use of Python 3.11 or higher, Poetry dependency management, and Pytest automation framework, are collected from GitHub. These programs are forked into the AstuteSource organization and added as Git submodules. Test suite compatibility is ensured across multiple operating systems.

Detection of Source Code Anti-Patterns: Static analysis tools, namely Chasten and MutMut, are utilized to identify and quantify code quality anti-patterns within the subject programs. This involves scanning for predefined patterns established in prior research, such as those correlated with low mutation scores. Additionally, configurations are made to detect code smells similar to those identified by PyNose.

Collection of Mutation Scores: Mutation testing tools, including Mutmut and Mutatest, are employed to gather mutation scores on a per-function basis. Configuration settings are adjusted to facilitate this data collection process, possibly utilizing the Hammet test automation framework for enhanced efficiency.

Unification of Data Sources: A stand-alone Python program is developed to merge data collected from static analysis and mutation testing tools. The unified dataset is structured in a tidy format and includes essential information for each subject program, function, detected anti-patterns, and mutation scores.

Calculation of Statistical Correlations: Statistical correlations, particularly at the function level, between the count of detected anti-patterns and mutation scores are computed using methodologies outlined in prior research. Correlation coefficients such as Spearman's rank correlation are determined and integrated into the unified dataset.

Training and Evaluation of Machine Learning Models: Following confirmation of statistical correlations, automated machine learning frameworks (e.g., AutoGluon, Auto-Sklearn) are utilized to develop predictive models using the unified dataset. Models are trained and evaluated using k-fold cross-validation to assess accuracy, precision, and effectiveness based on metrics like F1-score and Matthews correlation coefficient (MCC).

These methods provide a comprehensive framework for investigating the research questions while addressing potential challenges encountered during the research process.

## Using the Artifact

<!-- TODO: The result of your work will be the delivery of some type of artifact which will likely contain software programming solutions (i.e., Python code, HTML pages, or similar). To allow the user to experience and execute your artifact, you must first explain how to set up the initial conditions to run or use the artifact. Be sure to offer explicit details and instructions regarding the installation of the necessary foundational libraries, drivers, external software projects, containers and similar types of tertiary software which are involved in executing your artifact. Once these initial software installations have been completed, then you are asked to offer the necessary instructions for actually executing the artifact. For this, please provide all command line parameters or associated bash commands for execution. Please remember that users are unwilling to "figure-out" how to use code in absence of the essential instructions concerning the execution of project artifacts. -->

Due to time constraints, we were unable to fully complete the scope of the original proposed tool. However, we have developed a proof of concept artifact designed to predict mutation scores using Chasten and custom weights. To set up and use the artifact, follow these steps:

1. Ensure you are on the AlishPredict branch of the SEERS repository.

2. Navigate to the scripts\analyzer directory.

3. Run the command poetry install to install the necessary dependencies.

4. Clone the subject program into the demo folder.

5. Ensure you are back in the analyzer folder.

6. Execute the following command: `poetry run analyzer --search-path ChastenTest --chasten-config-path Config`

These steps will configure and run the artifact for predicting mutation scores using the specified parameters and settings.

## Results and Outcomes

<!-- TODO: Discuss the outcomes of your project in this section. Depending on the project type, the presented results and outcomes will vary. In some projects, you will be asked to present a theoretical analysis, and in others your experimental study and its results. In this section, you are also to demonstrate an enhanced version of your artifact by showing its capabilities and applications, in light of the evaluation metrics for assessing the artifact -->

Unfortunately, due to time constraints, we were unable to fully complete the scope of the original proposed tool. However, we have developed a proof of concept tool as a preliminary step towards achieving the intended functionality. We acknowledge that the current version may lack certain features and optimizations expected in the final tool. We encourage further development and refinement to realize the full potential of the envisioned tool.

The output of our tool on the Chasten codebase revealed several insights. Specifically, it successfully identified areas for potential improvement in code quality and highlighted specific code mutations. For instance, it detected over 100 instances of certain checks, ensuring their presence and correct definition. Additionally, various checks were performed, including assessments of nested conditions and loop iterations within functions, showcasing the tool's detailed analysis capabilities. Moreover, the tool calculated a predicted mutation score of 0.2258677840072424, providing a quantitative measure of the code’s test effectiveness. This score indicates the percentage of induced mutations the current test suite can detect, offering valuable insights for developers to enhance their code. The complete data is available in alish_result.json, offering a comprehensive report on each analyzed code element, enabling users to confirm mutation scores for specific patterns and functions, and assess the effectiveness of their test suites against potential code mutations.

The output of the artifact on the `Chasten` codebase:

```text
'chasten' already seems to be installed. Not modifying existing installation in '/home/student/.local/share/pipx/venvs/chasten'. Pass '--force' to force installation.

💫 chasten: Analyze the AST of Python Source Code
🔗 GitHub: https://github.com/gkapfham/chasten

✨ Configuration directory: Config

✨ Validated Config? Yes
✨ Validated Config/checks.yml? Yes

✨ Analyzing Python source code in: /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest

🎉 Performing 32 check(s):

  ✗ id: 'C001', name: 'class-definition', pattern: './/ClassDef', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/enumerations.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/constants.py - 10 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/results.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/debug.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/server.py - 1 matches
   = 25 total matches

  ✗ id: 'F001', name: 'all-function-definition', pattern: './/FunctionDef', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 11 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/util.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/createchecks.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 10 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/server.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 9 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configApp.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_debug.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_constants.py - 5 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_validate.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 16 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_database.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_util.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_main.py - 19 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configuration.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_checks.py - 11 matches
   = 174 total matches

  ✗ id: 'F002', name: 'dummy-test-non-test-function-definition', pattern: './/FunctionDef[not(contains(@name, "test_"))]', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 11 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 10 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/util.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/createchecks.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 10 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/server.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 9 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_main.py - 1 matches
   = 90 total matches

  ✗ id: 'CL001', name: 'dummy-test-single-nested-if', pattern: './/FunctionDef/body//If', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 17 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 5 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 7 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 10 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/util.py - 5 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/createchecks.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 38 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 11 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 13 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_constants.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_util.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_checks.py - 1 matches
   = 129 total matches

  ✗ id: 'CL002', name: 'dummy-test-double-nested-if', pattern: './/FunctionDef/body//If[ancestor::If and not(parent::orelse)]', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 15 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 3 matches
   = 32 total matches

  ✗ id: 'IMP001', name: 'import-from-star', pattern: '//ImportFrom/keyword[@name="from"]', min=1, max=10
   = 0 total matches

  ✗ id: 'RET001', name: 'explicit-return-in-init', pattern: '//FunctionDef[@name="init"]/body/Return', min=1, max=10
   = 0 total matches

  ✗ id: 'NONE001', name: 'none-comparison', pattern: '//Compare/left[@id="input_dirs"]/following-sibling::Compare/ops/NotEq | 
//Compare/comparators[@id="input_dirs"]/following-sibling::Compare/ops/NotEq', min=1, max=10
   = 0 total matches

  ✗ id: 'EXC001', name: 'no-exception-type', pattern: './/Try/ExceptHandler[not(ExceptHandler/type)]', min=1, max=10
   = 0 total matches

  ✗ id: 'BOOL001', name: 'boolean-comparison', pattern: '//Compare/ops/Is | //Compare/ops/Eq', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/util.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/createchecks.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 7 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 7 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configApp.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_debug.py - 9 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_constants.py - 10 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 23 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_util.py - 5 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_main.py - 16 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_checks.py - 16 matches
   = 117 total matches

  ✗ id: 'EXC001', name: 'no-exception-type', pattern: '//Try/ExceptHandler[not(ExceptHandler/type)]', min=1, max=10
   = 0 total matches

  ✗ id: 'ANNOT001', name: 'missing-annotations', pattern: '//FunctionDef[not(args/arg/annotation) or not(returns)]', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 11 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/util.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/createchecks.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 10 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/server.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 9 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configApp.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_debug.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_constants.py - 5 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_validate.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 16 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_database.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_util.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_main.py - 19 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configuration.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_checks.py - 11 matches
   = 174 total matches

  ✓ id: 'KF001', name: 'Key function', pattern: '//FunctionDef//Call/func/Attribute[@attr="keys"]', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 1 matches
   = 1 total matches

  ✗ id: 'MVKL001', name: 'Multi Value Key Literal', pattern: '//FunctionDef[@name="tp"]/body/Assign/value/Dict/keys/Name[preceding-sibling::Name/@id = @id]', min=1, max=10
   = 0 total matches

  ✗ id: 'AT001', name: 'Assert Tuple', pattern: '//FunctionDef[./body/Assert/test/Tuple]', min=1, max=10
   = 0 total matches

  ✗ id: 'LVITOI001', name: 'Loop variable iterates overrides iterator', pattern: '//FunctionDef/body/For[target/Name/@id = iter/Name/@id]', min=1, max=10
   = 0 total matches

  ✓ id: 'FLV001', name: 'Function uses loop variable', pattern: '//FunctionDef[body//comprehension/target/Name]', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 2 matches
   = 5 total matches

  ✗ id: 'F001', name: 'Nested Depth (Set value)', pattern: '//FunctionDef//FunctionDef/ancestor::*', min=1, max=10
   = 0 total matches

  ✗ id: 'F002', name: 'Number of conditions (if, if-else, and switch) in a Function', pattern: '//FunctionDef//If/following-sibling::If | //FunctionDef//If/following-sibling::Elif | 
//FunctionDef//If/following-sibling::Else', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 5 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 13 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 3 matches
   = 26 total matches

  ✗ id: 'CL001', name: 'The number of nested conditions (e.g., if{if{}}) in a Function', pattern: '//FunctionDef//If/descendant::If', min=1, max=1
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 1 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 17 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 6 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 3 matches
   = 46 total matches

  ✗ id: 'CL002', name: 'The number of nested condition-loops (e.g., if{for{}}) in a Function', pattern: '//FunctionDef//if//For', min=1, max=10
   = 0 total matches

  ✗ id: 'C002', name: 'The number of nested loop-conditions (e.g., for{if{}}) in a Function', pattern: '//FunctionDef[//(If/following-sibling::For | For/following-sibling::If)]', 
min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 11 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/util.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 10 matches
   = 45 total matches

  ✓ id: 'F001', name: 'The number of nested loop-conditions (e.g., for{for{}}) in a Function', pattern: '//FunctionDef//For[.//For]', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 2 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 3 matches
   = 5 total matches

  ✗ id: 'NOA001', name: 'number-of-assertions', pattern: '//FunctionDef[@type='str']/body/Assert', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configApp.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_debug.py - 16 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 3 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_constants.py - 9 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_validate.py - 9 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 34 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_util.py - 7 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_main.py - 30 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configuration.py - 8 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_checks.py - 16 matches
   = 140 total matches

  ✗ id: 'LOF001', name: 'count-test-method-lines', pattern: '//FunctionDef[@type='str' and starts-with(@name, 'test_')]/body/*', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configApp.py - 17 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_debug.py - 26 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 11 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_constants.py - 26 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 18 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_validate.py - 19 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 107 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_database.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_util.py - 17 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_main.py - 120 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configuration.py - 14 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_checks.py - 42 matches
   = 421 total matches

  ✗ id: 'CML001', name: 'count-method-lines', pattern: '//FunctionDef[@type='str']/body/* | //FunctionDef[@type='str']/body/Return', min=1, max=10
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configuration.py - 60 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/process.py - 16 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/validate.py - 12 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/output.py - 47 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/configApp.py - 26 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/util.py - 31 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/createchecks.py - 7 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/main.py - 112 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/filesystem.py - 61 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/database.py - 30 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/server.py - 13 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/chasten/checks.py - 33 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configApp.py - 17 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_debug.py - 26 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_process.py - 11 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_constants.py - 26 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_createchecks.py - 20 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_validate.py - 19 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_filesystem.py - 107 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_database.py - 4 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_util.py - 17 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_main.py - 122 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_configuration.py - 14 matches
    • /home/student/juniorsem/SEERS/scripts/analyzer/ChastenTest/chasten/tests/test_checks.py - 42 matches
   = 873 total matches

  ✗ id: 'TMIM001', name: 'test-methods-invoking-method', pattern: '//Assert[count(.//Call[func/Name/@id='test_function']) > 0]', min=1, max=10
   = 0 total matches

  ✗ id: 'DUCM001', name: ' notusingcontextmanager', pattern: '//*[starts-with(., 'with open')]', min=1, max=10
   = 0 total matches

  ✗ id: 'IF001', name: 'importfuture', pattern: '//ImportFrom[@module='__future']/alias[not(starts-with(@name, 'division') or starts-with(@name, 'absolute_import') or 
starts-with(@name, 'print_function') or starts-with(@name, 'unicode_literals'))]', min=1, max=10
   = 0 total matches

  ✗ id: 'F406', name: 'undefined-local-with-nested-import-star-usage', pattern: '//FunctionDef//ImportFrom[starts-with(@module, 'import') and @names=('*')]', min=1, max=10
   = 0 total matches

  ✗ id: 'F632', name: 'Use_of ==_to_compare_constant  ', pattern: '//function[@name='your_function_name']/*[your_xpath_condition]', min=1, max=10
   = 0 total matches

  ✗ id: 'F701', name: 'break_outside_loop', pattern: '//FunctionDef[BreakStmt[count(ancestor::For|ancestor::While|ancestor::If) = 0]]', min=1, max=10
   = 0 total matches

💻 3 / 32 checks passed (9.375%)


✨ Saved the file 'chasten-results-lazytracker-20240318134810-be9f98dad43e4cfaa654ca676ab77295.json'
😓 At least one check did not pass.
Predicted Score: 0.2258677840072424


Code analysis and mutation prediction complete!
Result is stored in file named alish_result.json
```

---

## Exemplar Projects Discussions

The department's project descriptions can be found at [https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects)

## Schedule

The schedule for this work can be found at [https://github.com/CMPSC-580-Allegheny-College-Spring-2024/classDocs?tab=readme-ov-file#schedule](https://github.com/CMPSC-580-Allegheny-College-Spring-2024/classDocs?tab=readme-ov-file#schedule)