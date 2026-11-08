---
layout: default
---

# DSC 180A Methodology Assignment 4

**Name:** Karthik Sankaran  
**Email:** ksankaran@ucsd.edu  
**Section / Domain:** Domain D20 (NLP / BabyLMs)  
**Mentor:** Prof. Alex Warstadt  

---

**What is the most interesting topic covered in your domain this quarter?**  
Getting to look under the hood of transformers and  pretraining a language model from scratch was interesting. It was interesting to see how choices like attention heads, masking strategies, and tokenization actually affect training, especially when working under a strict data limit.

**Describe a potential investigation you would like to pursue for your Quarter 2 Project.**  
I'd like to explore how pretraining on speech and prosody data compares to pretraining purely on text. Human children learn to talk by hearing tone, pauses, and pitch cues, not by reading written sentences. I want to see if feeding those acoustic patterns to a small model helps it learn grammar and sentence structure differently. 

**What is a potential change you’d make to the approach taken in your current Quarter 1 Project?**  

On the technical side, I want to move away from relying exclusively on autoregressive decoder-only models. We focused primarily on causal GPT-style setups in Q1, but for Q2 I want to experiment with encoder-only and encoder-decoder architectures to see if bidirectional context helps the model learn language.

I also want to rely less AI generated fixes and spend more time understanding each step of the pipeline manually. Earlier on, our team was faced with a steep learning curve which resulted in a lot of friction and sloppy collaboration. For Q2, I want to set up cleaner experiment tracking from day one, run smaller sanity checks before full training runs, and make sure everyone is organized and on the same page.

**What other techniques would you be interested in using in your project?**  
I'd like to experiment with curriculum learning where we starting training on simpler, shorter sentences (like child-directed speech) and gradually ramping up to longer, more complex text as the model learns. I'm also interested in testing teacher-student models or multi-task setups, where an audio model helps guide the language model during training so it doesn't have to figure out linguistic structure entirely on its own.