## 📝 Assignment 3 Instruction: Deep Learning for Blood-Cell Classification

-----

### **Overview**

[cite\_start]The goal of this final assignment is to evaluate your ability to apply deep learning knowledge and techniques to a real-world image classification task[cite: 5]. [cite\_start]You will design, implement, train, and evaluate a deep learning model to accurately classify microscopic images of different types of cells into their corresponding categories[cite: 6].

  * [cite\_start]**Due Date:** 30 November, 23:59[cite: 1]. [cite\_start]This is the final due date, and no extension will be granted[cite: 2, 3].
  * [cite\_start]**Objective:** Classify microscopic images of blood cells into eight categories[cite: 6, 29].
  * **Submission Components:** Technical Report (Task 1), Code (Task 2), and Model Performance Predictions (Task 3).
  * [cite\_start]**Techniques:** You are encouraged to apply any deep learning methods or architectures introduced during the semester, justifying your approach[cite: 7].

-----

### **Dataset Description**

[cite\_start]The dataset consists of real microscopic blood-cell images collected from a clinical laboratory[cite: 27].

  * [cite\_start]**Image Details:** Each image has a resolution of $360 \times 363$ pixels [cite: 20, 28] [cite\_start]and is in JPG format[cite: 28].
  * **Data Split:** You are provided with:
      * [cite\_start]**Training Images:** 3,200 images[cite: 29].
      * [cite\_start]**Testing Images:** 1,000 images[cite: 29].
  * [cite\_start]**Cell Categories:** The data covers eight major cell types (Figure 1 on Page 1 shows examples)[cite: 19, 29, 30]. [cite\_start]The file names in the training set contain the cell-type abbreviation (e.g., BA XXXX.jpg for Basophil)[cite: 35].
  * [cite\_start]**Class Mapping:** The mapping between class names and numerical IDs is defined in the file `class_map.json`[cite: 33]. [cite\_start]**Do not modify this file**[cite: 34].

| Class ID | Cell Type | Abbreviation |
| :---: | :--- | :--- |
| 0 | Basophil | (BA) [cite\_start][cite: 36] |
| 1 | Eosinophil | (EO) [cite\_start][cite: 36] |
| 2 | Erythroblast | (ERB) [cite\_start][cite: 36] |
| 3 | Immature Granulocyte | (IG) [cite\_start][cite: 36] |
| 4 | Lymphocyte | (LY) [cite\_start][cite: 36] |
| 5 | Monocyte | (MO) [cite\_start][cite: 36] |
| 6 | Neutrophil | (BNE) [cite\_start][cite: 36] |
| 7 | Platelet | |

-----

### **General Guidance and Requirements**

#### **Do's (Allowed)**

  * [cite\_start]Use any model architecture introduced in the Deep Learning Fundamentals (DLF) course, such as CNNs, RNNs, Transformers, Autoencoders, or large language models if appropriate[cite: 43].
  * [cite\_start]Explore and compare multiple network structures, loss functions, or training strategies[cite: 45].
  * [cite\_start]Use any training techniques covered, including optimizers (e.g., Adam, SGD), learning-rate scheduling, normalization (e.g., BatchNorm), and regularization (e.g., dropout)[cite: 46].
  * [cite\_start]**Data augmentation** is allowed and encouraged[cite: 47].
  * [cite\_start]Use open-source libraries like PyTorch, TensorFlow, scikit-learn, NumPy, or Pandas[cite: 48].
  * [cite\_start]Maintain clean, modular, and reproducible code (Jupyter Notebook is encouraged)[cite: 49].

#### **Don'ts (Forbidden)**

  * [cite\_start]**You must NOT use any pre-trained models or weights** (e.g., classifiers pre-trained on ImageNet or external datasets)[cite: 51].
  * [cite\_start]**You must NOT use any external labeled datasets** beyond the provided training data[cite: 52].
  * [cite\_start]You must NOT manually label, alter, or annotate any of the provided images in the **testing set**[cite: 54].
  * [cite\_start]You must NOT hard-code any results or predictions[cite: 55].
  * [cite\_start]You must NOT use any third-party APIs, pre-built AI services, or auto-training frameworks that automate model selection or hyperparameter tuning[cite: 57].

-----

### **Task Breakdown and Grading**

| Task | Description | Weight |
| :--- | :--- | :--- |
| **1** | Technical Report (up to 6 pages) | [cite\_start]15% [cite: 60, 66] |
| **2** | Code Implementation and Experiments | [cite\_start]10% [cite: 102] |
| **3** | Model Performance on Confidential Test Set | [cite\_start]10% [cite: 127, 128] |

#### **Task 1: Technical Report (15%)**

[cite\_start]The report must be presented using either the official **CVPR (two-column)** or **ICLR (one-column) $\LaTeX$ template**[cite: 61]. [cite\_start]**Do not modify any default settings** (font size, margins, etc.)[cite: 64].

  * [cite\_start]**Page Limit:** Must **not exceed 6 pages** (excluding references)[cite: 66]. [cite\_start]Content beyond 6 pages will not be marked, and each extra page incurs a 1-mark deduction[cite: 67, 68].
  * [cite\_start]**Submission:** A single PDF file must be submitted to GradeScope[cite: 70].
  * [cite\_start]**AI Use:** Generative AI tools are allowed for brainstorming, grammar checks, or proofreading, but **must not be used to generate full paragraphs, technical explanations, or any substantive part** of the report[cite: 71, 72].

| Section | Marks | Requirements |
| :--- | :--- | :--- |
| **Abstract & Introduction** | [cite\_start]2% [cite: 76] | Summarize the problem, motivation, dataset, approach, and key findings. [cite\_start]Clearly describe the problem, motivation, context, and outline the method[cite: 76, 77, 78]. |
| **Related Work** | [cite\_start]1% [cite: 80] | Summarize relevant previous studies/methods for image classification or blood-cell analysis. [cite\_start]Compare and justify design choices[cite: 80, 81]. |
| **Method** | [cite\_start]5% [cite: 82] | Detail your model architecture, algorithm, and training process. Select **one** DLF architecture as your main model and apply optimization/improvement techniques. [cite\_start]Explain structure and training for reproducibility[cite: 82, 83, 84, 85]. |
| **Experiments and Results** | [cite\_start]5% [cite: 87] | Describe experimental setup, dataset division, metrics, and parameters. Present results, including a comparison with **at least two baseline methods** (traditional ML or simpler NNs are acceptable). [cite\_start]Conduct a comprehensive **ablation study**[cite: 88, 89, 92]. |
| **Discussion** | [cite\_start]2% [cite: 94] | [cite\_start]Reflect on findings, discuss challenges, limitations, and suggest future work[cite: 94]. |
| **References** | N/A (Deductions possible) | Include all cited works using a consistent academic format. [cite\_start]Missing/incorrect citations may result in deductions[cite: 95, 96]. |
| **Template and Formatting** | N/A (Deductions possible) | Use the official CVPR or ICLR $\LaTeX$ template. [cite\_start]Failure to comply or manual modification of formatting parameters may result in deductions[cite: 99, 101]. |

#### **Task 2: Code (10%)**

[cite\_start]The code must be well-structured, clear, and able to reproduce all reported results[cite: 103, 104, 118]. [cite\_start]All analysis belongs in the report, not the code[cite: 106, 120].

| Section | Marks | Requirements |
| :--- | :--- | :--- |
| **Preprocessing** | [cite\_start]2% [cite: 107] | Implement techniques for data preparation (cleaning, normalization, splitting). [cite\_start]Brief visualizations are encouraged to assist in understanding the dataset[cite: 107, 108]. |
| **Model Implementation** | [cite\_start]4% [cite: 110] | [cite\_start]Implement your **main proposed method from scratch** using Python OOP in PyTorch or TensorFlow[cite: 110, 115]. [cite\_start]Include at least **two baseline models** (can use built-in/pre-trained modules for baselines)[cite: 113, 114]. |
| **Experiments** | [cite\_start]4% [cite: 117] | Code must align with the experiments/results in the report. Must show evidence that results were generated from actual implementation. [cite\_start]Should include an organized ablation study/controlled comparisons[cite: 117, 118, 119]. |
| **Code Structure and Organization** | N/A (Deductions possible) | Code must be cleanly structured, logically organized, and easy to navigate. [cite\_start]Poor structure or lack of readability may result in deductions[cite: 122, 125]. |

#### **Task 3: Model Performance (10%)**

[cite\_start]Your model's predictions on a confidential test set will be evaluated based on test accuracy and ranked among all students[cite: 128, 130].

  * [cite\_start]**Submission Format:** Submit a JSON file named **`prediction_labels.json`**[cite: 144].
      * [cite\_start]The file should map image filenames (sample ID) to the predicted class label (numerical ID)[cite: 137].
      * Example:
        ```json
        {
        [cite_start]"img_0.jpg": 0, [cite: 141]
        [cite_start]"img_1.jpg": 1, [cite: 142]
        [cite_start]"img_2.jpg": 2, [cite: 143]
        }
        ```
  * [cite\_start]**Submission Limit:** You are allowed to submit a **maximum of three times** to prevent overfitting[cite: 150]. [cite\_start]Additional submissions will not be recorded and will incur mark deductions[cite: 152].
  * [cite\_start]**Minimum Threshold:** Submissions below **50% accuracy** receive 0 marks[cite: 136].

| Ranking by Accuracy | Marks |
| :--- | :--- |
| Top 10% of students | [cite\_start]10 marks [cite: 132] |
| Top 20% of students | [cite\_start]8 marks [cite: 133] |
| Top 50% of students | [cite\_start]6 marks [cite: 134] |
| All other students achieving accuracy above the minimum threshold (50%) | [cite\_start]5 marks [cite: 135] |

-----

Would you like me to elaborate on any specific task, requirement, or constraint?