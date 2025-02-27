# UniOne

The papers related to this dataset will be submitted to ICDAR 2025. In order to meet the blind review requirements, the specific contact information will be made public on May 25, 2025.

The UniOne dataset has been released for the study of the entire process of document parsing in modern literature. The sample dataset can be accessed through the following link:

OneDrive (to be added in the future)

# Instructions

Note: The UniOne dataset can only be used for non-commercial research purposes. For scholars or organizations who wish to use the UniOne dataset, please first fill out this application form and send it to us via email (preferably using an institutional email so that we can quickly identify your information) (contact information to be provided). When submitting the application form to us, please list or attach 1-2 publications you have published in the past 5 years to indicate that you (or your team) have conducted research in related fields such as OCR, mathematical expression recognition, document image processing, or visual information extraction. At present, this dataset is only available free of charge to scholars in the aforementioned fields. After receiving your letter, we will quickly verify your information within two weeks and provide you with the download link and decompression password for the dataset.

In addition, if you have other plans, you can also collaborate with us and we will provide more datasets on this basis.

# License

The UniOne dataset should be used for non-commercial research purposes under the Creative Attribution NonCommercial NoDerivatives 4.0 International (CC BY-NC-ND 4.0) license.

# Dataset

Currently, document parsing technology is facing the problem of "task silos" caused by fragmented datasets. With the widespread application of deep learning in document understanding, the construction of a unified and shared dataset for collaborative development of upstream and downstream tasks has become an inevitable trend. We have built the first UniOne document dataset that supports the parsing of upstream and downstream tasks. By systematically integrating tasks such as layout analysis, text line detection and recognition, and table recognition, we have innovatively established a cross-task annotation dataset. This dataset: (1) at the layout analysis level, includes 236,790 paragraph-level annotations across 14,481 pages, covering 11 semantic categories; (2) at the text line detection level, based on the layout analysis data, further adds fine-grained annotations for 340,890 lines in 198,901 text paragraphs; (3) for complex scenarios, it introduces 8,000 challenging handwritten mathematical expressions, 18,717 printed mathematical formulas, 26,849 formula texts with unified recognition annotations, and 1,169 tables extracted from papers to fully support document content parsing. To our knowledge, this dataset is the first to achieve cross-task joint modeling from macro layouts to micro elements, breaking through the limitations of traditional single-task datasets and providing essential infrastructure for building the next generation of intelligent document parsing systems.

![fig1](https://github.com/user-attachments/assets/5bdaf5ab-707c-4292-a2dd-f409e4ca8ba8)


At the layout analysis level, the existing data sets generally have the problem of too coarse semantic granularity. Most mainstream annotation schemes focus on the positioning of basic layout elements (such as text blocks, tables, and graphics), but ignore the division of the internal hierarchical structure of documents. This defect directly leads to the fact that the generated information is difficult to meet the needs of high-level applications such as directory construction and knowledge map generation. To address this limitation, we propose a fine-grained annotation system, based on which we complete a total of 236,790 paragraph level annotations on 14,481 pages, and explicitly record the logical reading order of each element of the layout to retain its hierarchical information.

In terms of text line detection and recognition, the error accumulation effect of the traditional multi-stage pipeline architecture has become a bottleneck restricting the development of technology. Especially when dealing with documents containing mathematical formulas and special symbols, the separation of character segmentation and semantic understanding will significantly reduce the recognition accuracy. This study proposes a line level end-to-end deep learning framework that regards embedded formulas and their surrounding conventional text as a unified semantic unit. Based on the 198,901 text paragraphs of the previous layout analysis, 340890 line level annotations have been further completed, and a segment line two-level joint annotation dataset has been constructed. In addition, we have supplemented 8,000 handwritten mathematical formulas with an average sequence length of 63, 18,717 printed mathematical formulas with a sequence length of 64-512, 26,849 single line formula text unified recognition annotation dataset, and 1169 table datasets extracted from papers.

With the wide application of deep learning technology in the field of document understanding, it has gradually become a trend to build a unified and shared data set to achieve the collaborative development of upstream and downstream tasks. On the one hand, the shared dataset ensures the consistency of data distribution and annotation standards for different tasks. On the other hand, by constructing multi-level annotations such as layout structure, text line detection and recognition, and table recognition on a single sample at the same time, the in-depth information complementation and feature sharing between tasks are realized. Unione dataset is built based on this concept.
