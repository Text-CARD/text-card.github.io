# Temporal Scene-Text Calibrating and Distilling for Text-Video Retrieval

## [1/6]Abstract
Existing text-video retrieval (TVR) methods mainly focus on aligning single-modal video content with text queries, overlooking heterogeneous scene text in videos. While scene text offers fine-grained semantics for cross-modal matching, its effective utilization faces two critical challenges: **1)** The temporal density of scene text imposes substantial computational burdens, and **2)** Redundant scene text and irrelevant video frames hinder the learning of clear temporal clues for retrieval. In this paper, we propose a temporal scene-text calibrating and distilling (T-CARD) network to encode scene text efficiently while capturing clear temporal clues. Concretely, we first design a window-OCR captioner that aggregates abundant scene text in videos into condensed sentences to reduce computational complexity. Then, we leverage the heterogeneous scene text as a self-supervised signal to calibrate the synchronization between window-level OCR captions and frames-level video sequences. Furthermore, we devise a context temporal clue distillation to capture the complementarity and relevance among scene text and video frames, generating clear temporal clues for retrieval. Extensive experiments show T-CARD achieves SOTA results on two scene text TVR datasets and one traditional TVR dataset. **The source code and trained models will be released soon.**

## [2/6] Task Introduction

<div style="display: flex; justify-content: space-between;">
    <figure>
        <img src="images/intro.gng" alt="Introduction Image" style="width: 100%;">
    </figure>
</div>

*Figure 1: The progress of scene-text aware text-video retrieval.*

## [3/6] MODEL ARCHITECTURE
![T-CARD Model Architecture](images/T-CARD.png)

*Figure 1: Pipeline of the proposed **T-CARD**. Window-OCR captioner is leveraged to aggregate abundant scene text into condensed OCR captions. Heterogeneous semantics calibrating uses scene text in both video frames and OCR captions as a signal for self-supervised learning. Context temporal clue distilling assigns each modal query with a learnable clue to obtain a clear context temporal clue.*



<!-- <div style="display: flex; justify-content: space-between;">
    <figure>
        <video controls style="width: 100%;">
            <source src="video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </figure>
</div> -->

## [2/6] Retrieval Process

<div style="display: flex; justify-content: space-between;">
    <figure>
        <img src="images/fig_1.gif" alt="New Visualization" style="width: 100%;">
    </figure>
</div>

<!-- <div style="display: flex; justify-content: space-between;">
    <figure>
        <video controls style="width: 100%;">
            <source src="video2.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </figure>
</div> -->


## [5/6] Text→Video Retrieval (1/2)
![Text→Video Retrieval (1/2)](images/i2t_1.png)

## [5/6] Text→Video Retrieval (2/2)
![Text→Video Retrieval (2/2)](images/i2t_2.png)



