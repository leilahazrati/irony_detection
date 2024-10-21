# irony_detection
Description

This project addresses the task of profiling irony speech spreaders on social networks utilizing clustering and transformer-based models. The proposed methodology significantly enhances ironic author profiling by introducing a novel multi-step approach that encompasses comprehensive text cleaning, clustering, feature reduction, and weighted averaging, ultimately facilitating the construction of a robust author profile. A notable contribution of this work is the employment of two pre-trained language models at distinct stages of the process, which contrasts with the conventional approach of using a single language model or a combination of deep learning and traditional methodologies.

This dual-model strategy, in conjunction with multi-stage cleaning, adeptly addresses the diverse writing styles and non-standard expressions that are characteristic of social media texts. By clustering writings without the influence of an author's stylistic elements—systematically removed during the cleaning phase—only the essential, topic-driven content is preserved. This refinement allows for more accurate categorization of the author's writing and a deeper comprehension of irony within each thematic area, thereby enhancing classification performance.

The code has been executed on the PAN22 dataset; however, due to the dataset's private nature, its availability is restricted. Therefore, the dataset is not included in this repository. Interested users may access the dataset directly from the PAN website: 
https://pan.webis.de/clef22/pan22-web/author-profiling.html#data

 Furthermore, the PaLM model has been utilized in this code, having been accessed during a public availability period. Unfortunately, the checkpoint cannot be provided here due to the proprietary nature of the model.

#for download model
!wget "https://huggingface.co/conceptofmind/palm-2b/resolve/main/palm_2b_8k_v0.pt" -O "./PaLM/checkpoints/palm_2b_8k_v0.pt"
#https://github.com/conceptofmind/PaLM/
